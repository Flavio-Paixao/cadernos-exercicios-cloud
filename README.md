# Cadernos de Exercícios: Cloud e DevOps

Dois cadernos de exercícios para praticar **arquitetura AWS, Terraform, Docker e Kubernetes**, indo do **desenho para o código** e do **código para o desenho**, com problemas reais e gabarito comentado.

Montei esses cadernos para a minha própria preparação para a certificação **AWS Solutions Architect Associate** e para entrevistas técnicas. Estão aqui para quem também estiver estudando.

## Os cadernos

| Caderno | Exercícios | O que cobre |
| --- | --- | --- |
| [01 · Arquitetura e Terraform](pdf/01-arquitetura-e-terraform.pdf) | 33, em 6 níveis | VPC, subnets, NAT, Security Groups em cadeia, ALB e Auto Scaling, IAM, serverless, módulos, duas regiões, erros comuns do Terraform, falhas de arquitetura, cases completos e revisão no estilo da prova |
| [02 · Docker e Kubernetes](pdf/02-docker-e-kubernetes.pdf) | 23, em 4 níveis | Dockerfile multi-stage, Compose, Deployment, Service, probes, ConfigMap e Secret, rollout e rollback, Ingress e Gateway API, HPA, StatefulSet, e os erros mais comuns (ImagePullBackOff, CrashLoopBackOff, OOMKilled…) |

## Como usar

1. Imprima e tente cada exercício sozinho por 15 a 20 minutos.
2. Nos exercícios "código para desenho", desenhe à mão: caixas, setas e portas.
3. Só depois abra o gabarito, no fim de cada caderno.
4. Anote o erro, a causa e como resolveu.

## Regras do treino

- **Terraform:** só `init`, `fmt`, `validate` e `plan`. Nada de `apply` numa conta AWS: os exercícios não precisam criar recursos.
- **Kubernetes:** tudo roda localmente no [Kind](https://kind.sigs.k8s.io/), com custo zero. Ao terminar: `kind delete cluster`.
- **Nunca** coloque senhas ou tokens em código, Dockerfile, YAML ou no Git.

## Projetos relacionados

Os níveis avançados usam como base os meus projetos de estudo, validados com `terraform plan`:

- **Seguros Horizonte:** aplicação em 3 camadas, em 2 zonas.
- **Vitrine Modas:** e-commerce serverless orientado a eventos.
- **Banco Rio:** recuperação de desastre em 2 regiões.
- **StatusHub** e **MicroLink:** Docker e Kubernetes, em construção.

---

Flávio Paixão · [flaviopaixao.dev](https://flaviopaixao.dev) · AWS Certified Cloud Practitioner
