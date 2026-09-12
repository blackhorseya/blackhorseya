# Sean Zheng

<a href="https://blog.seancheng.space"><img src="https://img.shields.io/badge/Blog-blog.seancheng.space-0e75b6?style=flat-square&logo=hexo&logoColor=white" alt="Blog" /></a>
<a href="https://github.com/blackhorseya/resume"><img src="https://img.shields.io/badge/R%C3%A9sum%C3%A9-LaTeX-008080?style=flat-square&logo=latex&logoColor=white" alt="Résumé" /></a>
<a href="https://linkedin.com/in/chengchincheng"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="https://medium.com/@blackhorseya"><img src="https://img.shields.io/badge/Medium-000000?style=flat-square&logo=medium&logoColor=white" alt="Medium" /></a>
<a href="https://leetcode.com/blackhorseya"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
<img src="https://komarev.com/ghpvc/?username=blackhorseya&label=Profile%20views&color=0e75b6&style=flat-square" alt="Profile views" />

Backend and platform engineer. I build services in **Go** — domain first, Clean Architecture,
dependencies pointing inward — and spend the rest of my time on the infrastructure they run on.

Most of what I publish here is one of two kinds: a system built the way I think systems should be built,
or notes from learning something properly rather than quickly.

---

## How I build

These are the opinions that show up in almost every repo here, so they are worth stating directly:

| | |
|---|---|
| **Domain first** | The domain layer is written before the database and the framework, and does not import either. |
| **Behaviour, not bags of data** | `order.Cancel()` rather than `order.SetStatus(CANCELLED)`. Objects expose what they *do*. |
| **Always valid** | Fields are private, constructors validate. An object that exists is an object in a legal state. |
| **Errors are values** | Wrapped with context, matched with `errors.Is`/`errors.As`, never a panic as flow control. |
| **Explicit over clever** | The boring solution that the next reader understands beats the elegant one they have to decode. |

---

## Selected work

| Project | Stack | What it is |
|---|---|---|
| [**ekko**](https://github.com/blackhorseya/ekko) ![](https://img.shields.io/github/stars/blackhorseya/ekko?style=flat-square&label=) | Go | Todo list built to grow into a Jira-like issue tracker — workflows, collaboration, reporting. |
| [**golang-101**](https://github.com/blackhorseya/golang-101) ![](https://img.shields.io/github/stars/blackhorseya/golang-101?style=flat-square&label=) | Go | Working through Go properly: concurrency, generics, tooling, the standard library's sharp edges. |
| [**petlog**](https://github.com/blackhorseya/petlog) ![](https://img.shields.io/github/stars/blackhorseya/petlog?style=flat-square&label=) | Go · TypeScript | Full-stack health management for multi-pet households — Go API, TypeScript web, Terraform deploy. |
| [**godine**](https://github.com/blackhorseya/godine) ![](https://img.shields.io/github/stars/blackhorseya/godine?style=flat-square&label=) | Go | Online food ordering system, written as a deliberate exercise in Domain-Driven Design. |
| [**sion**](https://github.com/blackhorseya/sion) ![](https://img.shields.io/github/stars/blackhorseya/sion?style=flat-square&label=) | Go | Data analysis and integration platform for car rental firms. |
| [**ryze**](https://github.com/blackhorseya/ryze) | Go | Blockchain explorer for TON — querying blocks, transactions, and accounts. |
| [**go-ddd**](https://github.com/blackhorseya/go-ddd) | Go | Reference layout for the architecture above — so I stop re-deriving it per project. |
| [**memcached-operator**](https://github.com/blackhorseya/memcached-operator) · [**webscraper-operator**](https://github.com/blackhorseya/webscraper-operator) | Go | Kubernetes operators — learning the controller-runtime model by building real ones. |

---

## Stack

**Languages**

[![](https://skillicons.dev/icons?i=go,rust,ts,py)](https://skillicons.dev)

**Platform & infrastructure**

[![](https://skillicons.dev/icons?i=kubernetes,docker,terraform,gcp,aws,git)](https://skillicons.dev)

**Data & observability**

[![](https://skillicons.dev/icons?i=postgres,mongodb,redis,kafka,grafana,prometheus)](https://skillicons.dev)

**Practice** — Clean Architecture · DDD · trunk-based development · Conventional Commits

---

<img src="https://github-readme-streak-stats.herokuapp.com/?user=blackhorseya&theme=default&hide_border=true&date_format=M%20j%5B%2C%20Y%5D" alt="GitHub streak" />
