 <div align="center">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://scarfbench.github.io/site/assets/images/scarf-dark.png">
      <source media="(prefers-color-scheme: light)" srcset="https://scarfbench.github.io/site/assets/images/scarf-light.png">
      <img alt="ScarfBench Logo" width="800">
    </picture>
  </div>

<div align="center">
    <a href="https://scarfbench.github.io/site"><img src="https://img.shields.io/badge/docs-scarfbench.github.io%2Fsite-blue?style=for-the-badge" alt="Documentation"></a>
    <a href="https://scarfbench.github.io/site/leaderboard/"><img src="https://img.shields.io/badge/leaderboard-view%20results-orange?style=for-the-badge" alt="Leaderboard"></a>
  </div>
  
  **ScarfBench** is a comprehensive benchmark suite of Java applications across **Jakarta EE**, **Quarkus**, and **Spring** frameworks, designed to systematically evaluate AI agents' ability to migrate enterprise Java
  applications while preserving functionality, idiomatic patterns, and architectural integrity.

  > All applications have been manually converted and verified by experienced developers. Each implementation has undergone rigorous testing to ensure functional correctness, adherence to framework-specific idioms, and
  preservation of architectural integrity.


  ---

  ## Repositories

  | Repository | Description |
  |---|---|
  | [**benchmark**](https://github.com/scarfbench/benchmark) | The core benchmark suite — all application examples with Dockerfiles, Makefiles, and smoke tests |

  ---

  ## What's in the Benchmark?

  ScarfBench includes **two categories** of examples spanning **7 architectural layers** and **5 production-grade whole applications**, each implemented across all three target frameworks.

  ### Focused Examples

  Layer-specific demonstrations, each isolating a particular Java EE technology:

  | Layer | Examples | Key Technologies |
  |---|---|---|
  | **[Business Domain](https://ibm.github.io/scarfbench/business_domain/)** | [cart](https://github.com/scarfbench/benchmark/tree/main/benchmark/business_domain/cart), [converter](https://github.com/scarfbench/benchmark/tree/main/benchmark/business_domain/converter), [counter](https://github.com/scarfbench/benchmark/tree/main/benchmark/business_domain/counter), [helloservice](https://github.com/scarfbench/benchmark/tree/main/benchmark/business_domain/helloservice), [standalone](https://github.com/scarfbench/benchmark/tree/main/benchmark/business_domain/standalone) | EJBs (stateful, stateless, singleton), session beans |
  | **[Dependency Injection](https://ibm.github.io/scarfbench/dependency_injection/)** | [billpayment](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/billpayment), [decorators](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/decorators), [encoder](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/encoder), [guessnumber](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/guessnumber), [producerfields](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/producerfields), [producermethods](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/producermethods), [simplegreeting](https://github.com/scarfbench/benchmark/tree/main/benchmark/dependency_injection/simplegreeting) | CDI, qualifiers, interceptors, decorators, producers, observers |
  | **[Infrastructure](https://ibm.github.io/scarfbench/infrastructure/)** | [concurrency-jobs](https://github.com/scarfbench/benchmark/tree/main/benchmark/infrastructure/concurrency-jobs), [concurrency-taskcreator](https://github.com/scarfbench/benchmark/tree/main/benchmark/infrastructure/concurrency-taskcreator), [ejb-async](https://github.com/scarfbench/benchmark/tree/main/benchmark/infrastructure/ejb-async), [ejb-interceptor](https://github.com/scarfbench/benchmark/tree/main/benchmark/infrastructure/ejb-interceptor), [ejb-timersession](https://github.com/scarfbench/benchmark/tree/main/benchmark/infrastructure/ejb-timersession) | Managed executors, async EJBs, interceptors, timer services |
  | **[Persistence](https://ibm.github.io/scarfbench/persistence/)** | [address-book](https://github.com/scarfbench/benchmark/tree/main/benchmark/persistence/address-book), [order](https://github.com/scarfbench/benchmark/tree/main/benchmark/persistence/order), [roster](https://github.com/scarfbench/benchmark/tree/main/benchmark/persistence/roster) | JPA, CRUD, entity relationships, composite keys, JPQL |
  | **[Presentation](https://ibm.github.io/scarfbench/presentation/)** | [dukeetf](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/dukeetf), [dukeetf2](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/dukeetf2), [fileupload](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/fileupload), [hello-servlet](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/hello-servlet), [jaxrs-customer](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/jaxrs-customer), [jaxrs-hello](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/jaxrs-hello), [jaxrs-rsvp](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/jaxrs-rsvp), [mood](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/mood), [websocketbot](https://github.com/scarfbench/benchmark/tree/main/benchmark/presentation/websocketbot) | Servlets, JAX-RS, WebSockets, SSE, filters, listeners |

  ### Whole Applications

  Complete, production-grade systems demonstrating multi-layer coordination:

  | Application | Description |
  |---|---|
  | **[CargoTracker](https://ibm.github.io/scarfbench/cargotracker/)** ([code](https://github.com/scarfbench/benchmark/tree/main/benchmark/whole_applications/cargotracker)) | DDD cargo shipping tracker — Jakarta Faces, CDI, EJBs, JPA, REST, Batch, JMS. Implements Eric Evans' DDD patterns. |
  | **[Coffee Shop](https://ibm.github.io/scarfbench/coffee_shop/)** ([code](https://github.com/scarfbench/benchmark/tree/main/benchmark/whole_applications/coffee-shop)) | Event-driven microservices (Orders, Barista, Kitchen) via Kafka. MicroProfile, reactive messaging, eventual consistency. |
  | **[DayTrader](https://ibm.github.io/scarfbench/daytrader/)** ([code](https://github.com/scarfbench/benchmark/tree/main/benchmark/whole_applications/daytrader)) | High-performance stock trading benchmark — stateless session beans, JPA optimistic locking, transaction management. |
  | **[PetClinic](https://ibm.github.io/scarfbench/petclinic/)** ([code](https://github.com/scarfbench/benchmark/tree/main/benchmark/whole_applications/petclinic)) | Veterinary clinic management — Jakarta Faces (PrimeFaces), complex JPA relationships, CDI, Bean Validation. |
  | **[RealWorld](https://ibm.github.io/scarfbench/realworld/)** ([code](https://github.com/scarfbench/benchmark/tree/main/benchmark/whole_applications/realworld)) | Medium.com clone (Conduit) — MicroProfile JWT, JAX-RS, JPA, Testcontainers integration tests. |

  ---
  Links:

  - Documentation & Guide: [scarfbench.github.io/site](https://scarfbench.github.io/site)
  - Quickstart: [scarfbench.github.io/site/quickstart](https://scarfbench.github.io/site/quickstart)
  - Leaderboard: [scarfbench.github.io/site/leaderboard](https://scarfbench.github.io/site/leaderboard)
  - Submit Your Agent Results: [scarfbench.github.io/site/submit](https://scarfbench.github.io/site/submit)
  - Contributing Guide: [CONTRIBUTING.md](CONTRIBUTING.md)
  - Citation: [scarfbench.github.io/site/citation](https://scarfbench.github.io/site/citation)
