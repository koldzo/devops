<h3 align="left">Requirements</h3>
The following is a list of requirements:
<ul>
<li>Docker</li>
<p>
<a href="https://docs.docker.com/engine/install/ubuntu/" target="_blank">Install Docker Engine on Ubuntu</a>
</p>
<li>Docker compose</li>
<p>
<a href="https://docs.docker.com/compose/install/" target="_blank">Install Docker Compose</a>
</p>
</ul>
<hr>
<h3 align="left">Run the application with docker compose</h3>
<ul>
<li>
Clone the repo<br>
<code>git clone git@github.com:koldzo/devops.git</code>
</li>
<li>
Navigate to dir<br>
<code>cd devops</code>
</li>
<li>
Check credentials in environment file in <b>.env</b><br>
for default you do not change env credentials<br>
<p>
It is not a practice to commit data for .env, due to this task, the .env fille will be commmited to show my work.</p>
</li>
<li>
Run docker compose<br>
<code>docker-compose up</code> or <code>docker-compose up -d</code> (if you install standalone docker-compose) OR <br>
<code>docker compose up</code> or <code>docker compose up -d</code> (if you install compose plugin) <br>
- <code>-d</code>  flag runs containers in background
</li>
<li>
Once all services are running, for health check execute 
<code>
bash <(curl -s https://raw.githubusercontent.com/kkenan/basic-microservices/master/health_check.sh)
</code>
</li>
</ul>
App Ports:
<ul>
<li>Java App - 8080 </li>
<li>Node App - 8081 </li>
<li>PostgreSQL - 5432 </li>
</ul>
<hr>

<h4 align="left">Connect with me:</h4>
<p align="left">
<a href="https://linkedin.com/in/https://www.linkedin.com/in/jasminkoldzo/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="https://www.linkedin.com/in/jasminkoldzo/" height="30" width="40" /></a>
</p>
