<h1>🚀 Kubernetes: From Zero To Cloud - Kurs Uygulamaları ve Ödevler</h1>

<p>Bu depo, Rayan Slim tarafından hazırlanan <strong>"Kubernetes: From Zero To Cloud"</strong> kursu boyunca tamamladığım ödevleri, pratik uygulamaları ve YAML yapılandırma dosyalarını içermektedir.</p>

<hr>

<h2>📖 Proje Hakkında</h2>
<p>Bu repository, Kubernetes mimarisini anlamak ve modern yazılım altyapılarında konteyner orkestrasyonunu uygulamalı olarak öğrenmek amacıyla oluşturulmuştur. Depodaki her bir dosya veya klasör, kursta işlenen belirli bir Kubernetes objesinin (Pod, Deployment, Service vb.) çalışma mantığını pekiştirmek için yazılmış yapılandırma dosyalarını barındırır.</p>

<h2>🎯 Temel Kazanımlar</h2>
<p>Rayan Slim'in kursu aracılığıyla elde edilen temel yetkinlikler ve öğrenim çıktıları şunlardır:</p>
<ul>
    <li><strong>🏗️ Kubernetes Mimarisini Kavrama:</strong> Cluster bileşenlerinin, Node ve Container yapılarının arka plandaki çalışma mekanizması.</li>
    <li><strong>📈 Uygulama Dağıtımı ve Ölçeklendirme:</strong> Deployments ve ReplicaSets kullanılarak uygulamaların kesintisiz (zero-downtime) güncellenmesi ve ihtiyaç anında ölçeklendirilmesi.</li>
    <li><strong>🌐 Ağ ve İletişim Yönetimi:</strong> Services (ClusterIP, NodePort, LoadBalancer) ve Ingress kaynakları aracılığıyla Pod'lar arası ve dış dünya ile iletişimin güvenli bir şekilde yapılandırılması.</li>
    <li><strong>💾 Durum ve Veri Yönetimi (Storage):</strong> Volumes, Persistent Volumes (PV) ve Persistent Volume Claims (PVC) ile kalıcı veri depolama özelliklerinin entegre edilmesi.</li>
    <li><strong>🔐 Yapılandırma ve Güvenlik:</strong> Uygulama ortam değişkenlerinin (ConfigMap) ve hassas verilerin (Secret) koddan bağımsız, güvenli bir şekilde yönetilmesi.</li>
    <li><strong>📜 Deklaratif Yönetim:</strong> Tüm altyapı süreçlerinin YAML dosyaları üzerinden deklaratif bir yaklaşımla ("Infrastructure as Code" prensibiyle) tasarlanması ve uygulanması.</li>
</ul>

<hr>

<h2>⚙️ Kurulum ve Kullanım</h2>
<p>Bu depoda paylaşılan kodları ve ödev uygulamalarını kendi bilgisayarınızda test etmek için aşağıdaki adımları izleyebilirsiniz.</p>

<h3>🛠️ Gereksinimler</h3>
<p>Çalıştırma ortamınızı hazırlamak için aşağıdaki araçların bilgisayarınızda kurulu olması gerekmektedir:</p>
<ul>
    <li>🐳 <a href="https://docs.docker.com/get-docker/" target="_blank">Docker</a></li>
    <li>☸️ <a href="https://minikube.sigs.k8s.io/docs/start/" target="_blank">Minikube</a> (veya Docker Desktop Kubernetes eklentisi)</li>
    <li>⌨️ <a href="https://kubernetes.io/docs/tasks/tools/" target="_blank">kubectl</a> komut satırı aracı</li>
</ul>

<h3>🚀 Adımlar</h3>
<ol>
    <li>
        <strong>📥 Depoyu Klonlayın:</strong>
<pre><code>git clone https://github.com/KULLANICI_ADIN/REPO_ADIN.git
cd REPO_ADIN</code></pre>
    </li>
    <li>
        <strong>📂 İlgili Bölüme Gidin:</strong>
        <p>İncelemek veya çalıştırmak istediğiniz konunun klasörüne geçiş yapın (Örn: <code>01-pods</code>).</p>
<pre><code>cd 01-pods</code></pre>
    </li>
    <li>
        <strong>⚡ Konfigürasyonu Uygulayın:</strong>
        <p>YAML dosyasını lokal Kubernetes cluster'ınıza dağıtmak için <code>kubectl apply</code> komutunu kullanın.</p>
<pre><code>kubectl apply -f &lt;dosya-adi&gt;.yaml</code></pre>
    </li>
    <li>
        <strong>🔍 Durumu Kontrol Edin:</strong>
        <p>Kaynakların başarıyla oluşturulduğunu ve düzgün çalıştığını doğrulamak için aşağıdaki komutları kullanabilirsiniz:</p>
<pre><code>kubectl get pods
kubectl get services
kubectl get deployments</code></pre>
    </li>
    <li>
        <strong>🧹 Ortamı Temizleme:</strong>
        <p>İncelemeniz bittikten sonra sistem kaynaklarını serbest bırakmak için yapılandırmayı cluster'dan kaldırın:</p>
<pre><code>kubectl delete -f &lt;dosya-adi&gt;.yaml</code></pre>
    </li>
</ol>
