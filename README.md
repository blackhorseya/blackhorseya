<div align="center">

# Sean Zheng

**Backend &amp; platform engineer** &nbsp;·&nbsp; Go &nbsp;·&nbsp; Kubernetes &nbsp;·&nbsp; Clean Architecture

<a href="https://blog.seancheng.space"><img height="22" src="https://img.shields.io/badge/Blog-blog.seancheng.space-0e75b6?style=flat-square&logo=hexo&logoColor=white" alt="Blog" /></a>
<a href="https://github.com/blackhorseya/resume"><img height="22" src="https://img.shields.io/badge/R%C3%A9sum%C3%A9-008080?style=flat-square&logo=latex&logoColor=white" alt="Résumé" /></a>
<a href="https://linkedin.com/in/chengchincheng"><img height="22" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://medium.com/@blackhorseya"><img height="22" src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" alt="Medium" /></a>
<a href="https://leetcode.com/blackhorseya"><img height="22" src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
<img height="22" src="https://komarev.com/ghpvc/?username=blackhorseya&label=Views&color=0e75b6&style=flat-square" alt="Profile views" />

</div>

<br />

I build services in **Go** — domain first, Clean Architecture, dependencies pointing inward — and
spend the rest of my time on the infrastructure they run on.

Most of what I publish here is one of two kinds: a system built the way I think systems should be
built, or notes from learning something properly rather than quickly.

---

## How I build

<table>
<tr>
<td width="210"><b>Domain first</b></td>
<td>The domain layer is written before the database and the framework, and does not import either.</td>
</tr>
<tr>
<td><b>Behaviour, not bags of data</b></td>
<td><code>order.Cancel()</code> rather than <code>order.SetStatus(CANCELLED)</code>. Objects expose what they <i>do</i>.</td>
</tr>
<tr>
<td><b>Always valid</b></td>
<td>Fields are private, constructors validate. An object that exists is an object in a legal state.</td>
</tr>
<tr>
<td><b>Errors are values</b></td>
<td>Wrapped with context, matched with <code>errors.Is</code>/<code>errors.As</code>, never a panic as flow control.</td>
</tr>
<tr>
<td><b>Explicit over clever</b></td>
<td>The boring solution that the next reader understands beats the elegant one they have to decode.</td>
</tr>
</table>

---

## Selected work

<table>
<tr>
<td width="150"><a href="https://github.com/blackhorseya/ekko"><b>ekko</b></a><br /><sub>Go</sub></td>
<td>Todo list built to grow into a Jira-like issue tracker — workflows, collaboration, reporting.</td>
<td width="90" align="right"><img height="20" src="https://img.shields.io/github/stars/blackhorseya/ekko?style=flat-square&label=&color=444" alt="stars" /></td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/golang-101"><b>golang-101</b></a><br /><sub>Go</sub></td>
<td>Working through Go properly: concurrency, generics, tooling, the standard library's sharp edges.</td>
<td align="right"><img height="20" src="https://img.shields.io/github/stars/blackhorseya/golang-101?style=flat-square&label=&color=444" alt="stars" /></td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/petlog"><b>petlog</b></a><br /><sub>Go · TypeScript</sub></td>
<td>Full-stack health management for multi-pet households — Go API, TypeScript web, Terraform deploy.</td>
<td align="right"><img height="20" src="https://img.shields.io/github/stars/blackhorseya/petlog?style=flat-square&label=&color=444" alt="stars" /></td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/godine"><b>godine</b></a><br /><sub>Go</sub></td>
<td>Online food ordering system, written as a deliberate exercise in Domain-Driven Design.</td>
<td align="right"><img height="20" src="https://img.shields.io/github/stars/blackhorseya/godine?style=flat-square&label=&color=444" alt="stars" /></td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/sion"><b>sion</b></a><br /><sub>Go</sub></td>
<td>Data analysis and integration platform for car rental firms.</td>
<td align="right"><img height="20" src="https://img.shields.io/github/stars/blackhorseya/sion?style=flat-square&label=&color=444" alt="stars" /></td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/go-ddd"><b>go-ddd</b></a><br /><sub>Go</sub></td>
<td>Reference layout for the architecture above — so I stop re-deriving it per project.</td>
<td align="right"></td>
</tr>
</table>

<details>
<summary><b>More</b> — Kubernetes operators, blockchain, market data</summary>
<br />
<table>
<tr>
<td width="150"><a href="https://github.com/blackhorseya/ryze"><b>ryze</b></a><br /><sub>Go</sub></td>
<td>Blockchain explorer for TON — querying blocks, transactions, and accounts.</td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/memcached-operator"><b>memcached-operator</b></a><br /><sub>Go</sub></td>
<td>Kubernetes operator — learning the controller-runtime model by building a real one.</td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/webscraper-operator"><b>webscraper-operator</b></a><br /><sub>Go</sub></td>
<td>Second operator, non-trivial reconcile loop.</td>
</tr>
<tr>
<td><a href="https://github.com/blackhorseya/fugle-marketdata-go"><b>fugle-marketdata-go</b></a><br /><sub>Go</sub></td>
<td>Market data client — intake layer for building trading systems end to end.</td>
</tr>
</table>
</details>

---

## Stack

<table>
<tr>
<td width="180" align="right"><b>Languages</b></td>
<td><a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=go,rust,ts,py" alt="Go, Rust, TypeScript, Python" /></a></td>
</tr>
<tr>
<td align="right"><b>Platform</b></td>
<td><a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=kubernetes,docker,terraform,gcp,aws,git" alt="Kubernetes, Docker, Terraform, GCP, AWS, Git" /></a></td>
</tr>
<tr>
<td align="right"><b>Data &amp; observability</b></td>
<td><a href="https://skillicons.dev"><img src="https://skillicons.dev/icons?i=postgres,mongodb,redis,kafka,grafana,prometheus" alt="PostgreSQL, MongoDB, Redis, Kafka, Grafana, Prometheus" /></a></td>
</tr>
<tr>
<td align="right"><b>Practice</b></td>
<td>Clean Architecture &nbsp;·&nbsp; DDD &nbsp;·&nbsp; trunk-based development &nbsp;·&nbsp; Conventional Commits</td>
</tr>
</table>

---

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=blackhorseya&theme=dark&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=58A6FF" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=blackhorseya&theme=default&hide_border=true" alt="GitHub streak" />
</picture>
</div>
