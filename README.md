<h1>🐳 Containerisation & Déploiement Microservices – Spring Boot, Angular, Docker, Docker Compose</h1>

<h2>📘 Description générale</h2>
<p>
Ce projet démontre deux cas d’usage concrets liés à la containerisation et au déploiement d’applications Java/Angular :
</p>

<ol>
  <li><strong>Containerisation d'une application monolithique Spring Boot + Angular + PostgreSQL avec Docker & Docker Compose</strong></li>
  <li><strong>Déploiement d'une architecture microservices avec Spring Cloud, Docker & Docker Compose</strong></li>
</ol>

<hr>

<h2>📦 Partie 1 – Containerisation d'une Application Full Stack (Spring Boot + Angular + PostgreSQL)</h2>

<h3>🧱 Composants du projet</h3>
<ul>
  <li><strong>Frontend :</strong> Angular</li>
  <li><strong>Backend :</strong> Spring Boot REST API</li>
  <li><strong>Base de données :</strong> PostgreSQL</li>
  <li><strong>Chatbot IA :</strong> Intégration simple avec un service de chatbot (placeholder)</li>
  <li><strong>Infrastructure :</strong> Docker, Docker Compose</li>
</ul>

<h3>🚀 Étapes clés</h3>
<ol>
  <li>Création des <code>Dockerfile</code> pour Angular et Spring Boot</li>
  <li>Création d’un <code>docker-compose.yml</code> pour orchestrer les conteneurs</li>
  <li>Configuration du <code>application.properties</code> pour PostgreSQL</li>
  <li>Utilisation de <code>ng build --prod</code> pour builder l'app Angular dans Spring</li>
</ol>

<h3>📂 Arborescence simplifiée</h3>
<pre>
/frontend
  └── Dockerfile

/backend
  └── Dockerfile

/docker-compose.yml
</pre>

<h3>▶️ Lancer les conteneurs</h3>
<pre><code>
docker-compose up --build
</code></pre>

---

<h2>🧩 Partie 2 – Déploiement d'une Architecture Microservices avec Docker Compose</h2>

<h3>🧱 Composants Microservices</h3>
<ul>
  <li><strong>Service Discovery :</strong> Eureka</li>
  <li><strong>API Gateway :</strong> Spring Cloud Gateway</li>
  <li><strong>Config Server :</strong> Spring Cloud Config</li>
  <li><strong>Services métiers :</strong> Customer Service, Inventory Service...</li>
  <li><strong>Keycloak :</strong> Authentification et autorisation (OpenID Connect)</li>
  <li><strong>Base de données :</strong> PostgreSQL / MySQL selon les services</li>
</ul>

<h3>🚀 Étapes de déploiement</h3>
<ol>
  <li>Création de <code>Dockerfile</code> pour chaque microservice</li>
  <li>Utilisation d’un <code>docker-compose.yml</code> global pour tout orchestrer</li>
  <li>Configuration de <code>volumes</code>, <code>networks</code>, <code>depends_on</code></li>
  <li>Communication entre services via les noms de service définis dans Compose</li>
  <li>Sécurisation des endpoints avec Keycloak</li>
</ol>

<h3>📂 Exemple d’arborescence</h3>
<pre>
/config-server
/customer-service
/inventory-service
/eureka-discovery
/api-gateway
/keycloak
/docker-compose.yml
</pre>

<h3>▶️ Lancer l’architecture complète</h3>
<pre><code>
docker-compose up --build
</code></pre>

---

<h2>📑 Conclusion</h2>
<p>
Ce projet montre deux niveaux d’intégration avec Docker :
</p>
<ul>
  <li>✅ Containerisation d’une application monolithique full stack</li>
  <li>✅ Déploiement complet d’un système distribué microservices</li>
</ul>
<p>
Ces travaux démontrent la maîtrise des outils de conteneurisation et d’orchestration, essentiels pour le DevOps et les architectures cloud-native modernes.
</p>
