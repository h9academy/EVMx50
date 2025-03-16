# `EVMx50`

Curso de blockchain y smart contracts con Solidity y Vyper. Usando **[Cyfrin Updraft](https://updraft.cyfrin.io) como referencia y guía de estudio**. Enfocado a capas 2 de Ethereum como Polygon o Base.

## Cursos

Según preferencia se eligirá entre Solidity o Vyper como lenguaje de programación para desarrollar smart contracts. Con Solidity el enfoque será el desarrollo de apps mientras que con Vyper (y Python) además de apps se aplicará análisis de datos.

Los cursos de [Cyfrin Updraft](https://updraft.cyfrin.io) que usaremos como guía de estudio son gratuitos y se pueden completar en cualquier momento.

Es recomendable entender los conceptos de "Blockchain Basics" para el correcto aprovechamiento de los cursos de Solidity y Vyper. Este es el contenido que se dictará semanalmente en las lectures para tener fundamentos teóricos sólidos al momento de desarrollar los proyectos. Se le dará prioridad a programar desde el primer día (ver cursos de Solidity o Vyper en orden) mientras que progresivamente dominaremos los fundamentos semana a semana.

Otra recomendación es saber usar **Git y GitHub** para llevar el control de versiones en los proyectos, especialmente cuando se usen frameworks como Foundry o Moccasin.

La **línea de comandos**, especialmente con **Linux**, es también necesaria para desarrollar software.

[Blockchain Basics](https://updraft.cyfrin.io/courses/blockchain-basics) **[ 3hrs + 23 lessons + 1 project ]**

> Introductory blockchain developer course. Learn how blockchains and smart contracts work, and how to sign your first transaction. Whether you're new or are a seasoned developer, there's something here for you.

### Solidity

Si no sabes por dónde empezar, tomar esta ruta. Se dominará el desarrollo de apps decentralizadas para la web3.

[Solidity Smart Contract Development](https://updraft.cyfrin.io/courses/solidity) **[ 5hrs + 65 lessons + 3 projects ]**

> Start here if you're new to writing smart contracts! Learn Solidity programming language and smart contract development from industry-leading experts. Kickstart your career as a web3 developer.

[Foundry Fundamentals](https://updraft.cyfrin.io/courses/foundry) **[ 10hrs + 112 lessons + 3 projects ]**

> Learn Foundry for Solidity and level up your Solidity developer skills. Discover advanced web3 development concepts and tools in the Foundry Fundamentals course. Learn Foundry Forge and Anvil, Chainlink Blockchain oracles, smart contract testing, and how to spin up local networks.

[Advanced Foundry](https://updraft.cyfrin.io/courses/advanced-foundry) **[ 13hrs + 154 lessons + 4 projects ]**

> Learn advanced Foundry for Solidity smart contract development. Master web3 development techniques to write, deploy, test, optimize, and interact with your smart contracts using industry-standard tools. Lessons taught by the top smart contracts engineers in web3.

### Vyper

Para mejor integración con data science diseñamos el curso de Vyper y Python.

[Introduction to Python and Vyper](https://updraft.cyfrin.io/courses/intro-python-vyper-smart-contract-development) **[ 6hrs + 75 lessons + 4 projects ]**

> Start your journey as a Python and Vyper smart contract developer. Learn how to write, deploy, and interact with Python based smart contracts using the Vyper programming language. Learn how to build your decentralized applications and kickstart your career as a web3 developer.

[Intermediate Python and Vyper](https://updraft.cyfrin.io/courses/intermediate-python-vyper-smart-contract-development) **[ 14hrs + 174 lessons + 6 projects ]**

> Learn intermediated Python smart contract development using Vyper and level up your skills as a smart contract developer. This course will teach you how to test your Python based Vyper smart contracts, how to deploy contracts on ZKsync using Moccasin, the first web3 development framework to natively support ZKsync ERA, and launch your first cryptocurrency!

## Guía de Aprendizaje por Temas

### Solidity

1. **Fundamentos**: Comienza con [Solidity Smart Contract Development](https://updraft.cyfrin.io/courses/solidity) para aprender la sintaxis básica y conceptos fundamentales.
2. **Desarrollo Avanzado**: Continúa con [Foundry Fundamentals](https://updraft.cyfrin.io/courses/foundry) y [Advanced Foundry](https://updraft.cyfrin.io/courses/advanced-foundry) para dominar patrones de diseño y optimización.
3. **Recursos Adicionales**:
   - [Solidity by Example](https://solidity-by-example.org/)
   - [CryptoZombies](https://cryptozombies.io/)
   - [Documentación oficial de Solidity](https://docs.soliditylang.org/)
4. **Conceptos Lógicos Aplicados a Solidity**:
   - **Lógica Proposicional en Smart Contracts**:
     - Uso de operadores lógicos (`&&`, `||`, `!`) para construir condiciones de seguridad en modificadores
     - Simplificación de expresiones booleanas para reducir costos de gas en validaciones
     - Aplicación de leyes de De Morgan para optimizar condiciones complejas en funciones `require()`
     - Manejo de precedencia de operadores en expresiones condicionales para evitar bugs de seguridad
   - **Razonamiento Algorítmico en la EVM**:
     - Análisis del flujo de ejecución en funciones para prevenir reentrancy attacks
     - Modelado de transiciones de estado en mappings y estructuras de datos complejas
     - Verificación formal de invariantes en bucles para evitar desbordamientos y underflows
     - Optimización de operaciones de almacenamiento (SSTORE/SLOAD) mediante análisis lógico
5. **Ejercicios de Pensamiento Lógico para Solidity**:
   - **Escenarios Prácticos de Contratos**:
     - Implementación de mecanismos de votación con validación de quórum usando `mapping(address => bool)` y contadores
     - Diseño de sistemas de control de acceso con roles jerárquicos usando herencia y modificadores
     - Creación de esquemas de vesting de tokens con bloqueos temporales usando timestamps y bloques
     - Desarrollo de circuitos de pausa de emergencia con múltiples condiciones de activación
   - **Patrones de Resolución en Solidity**:
     - Refactorización de condiciones anidadas (`if` dentro de `if`) en expresiones más eficientes
     - Identificación de dependencias circulares entre contratos que pueden causar deadlocks
     - Eliminación de comprobaciones redundantes para optimizar gas en funciones frecuentemente llamadas
     - Análisis de casos extremos en operaciones matemáticas para prevenir vulnerabilidades de overflow
6. **Metodología de Desarrollo Seguro**:
   - **Técnicas de Análisis Lógico**:
     - Descomposición de funciones complejas en funciones más pequeñas y verificables
     - Aplicación de técnicas de optimización de gas mediante simplificación lógica de condiciones
     - Identificación de race conditions a través del análisis de flujo de transacciones
     - Modelado de ataques mediante árboles de decisión para identificar vulnerabilidades
   - **Ejercicios Prácticos de Seguridad**:
     - Implementación de sistemas de votación resistentes a ataques de flash loans
     - Desarrollo de mecanismos de control de acceso con timelock para operaciones críticas
     - Diseño de circuitos de pausa con múltiples signatarios y condiciones de activación
     - Optimización de verificaciones en bucles para reducir costos de gas sin comprometer seguridad

> **Nota para Desarrolladores**: En Solidity, la lógica no es solo una herramienta teórica sino una necesidad práctica. Cada operación tiene un costo de gas, y cada error lógico puede resultar en pérdidas financieras reales. Desarrollar la capacidad de descomponer problemas complejos en pasos lógicos verificables no solo mejora la calidad del código, sino que es esencial para la seguridad de los fondos gestionados por los contratos. Las vulnerabilidades más costosas en la historia de Ethereum han sido resultado de fallos lógicos aparentemente simples.

### DAOs (Organizaciones Autónomas Descentralizadas)

1. **Conceptos Básicos**: Estudia los fundamentos de gobernanza en blockchain y votación on-chain.
2. **Frameworks**:
   - [OpenZeppelin Governor](https://docs.openzeppelin.com/contracts/4.x/api/governance)
   - [Nouns Builder](https://builder-docs.vercel.app/)
   - [Compound Governor](https://docs.compound.finance/v2/governance/)
3. **Proyectos Prácticos**:
   - Implementa un sistema de votación simple
   - Crea una DAO con tesorería y propuestas
   - Estudia el código de [Nouns DAO](https://github.com/nounsDAO/nouns-monorepo)

### Ethereum

1. **Arquitectura**: Comprende el funcionamiento de la EVM (Ethereum Virtual Machine).
2. **Transacciones y Gas**: Aprende sobre el modelo de ejecución y optimización de gas.
3. **Recursos**:
   - [Ethereum Whitepaper](https://ethereum.org/en/whitepaper/)
   - [Ethereum Yellow Paper](https://ethereum.github.io/yellowpaper/paper.pdf)
   - [Ethereum Book](https://github.com/ethereumbook/ethereumbook)
4. **Herramientas**:
   - [Etherscan](https://etherscan.io/) para explorar transacciones
   - [Remix IDE](https://remix.ethereum.org/) para desarrollo rápido

### Capas 2 (Base, Polygon, etc.)

1. **Fundamentos de Escalabilidad**: Comprende los desafíos de escalabilidad en Ethereum.
2. **Tipos de Soluciones L2**:
   - Rollups (Optimistic y ZK)
   - Sidechains
   - State channels
3. **Base (L2 de Coinbase)**:
   - [Documentación oficial de Base](https://docs.base.org/)
   - [Base Camp](https://base.org/camp) - Programa de aprendizaje
   - [Onboarding para desarrolladores](https://docs.base.org/guides/deploy-smart-contracts)
4. **Polygon**:
   - [Documentación de Polygon](https://docs.polygon.technology/)
   - [Polygon Academy](https://academy.polygon.technology/)

### Oráculos (Chainlink)

1. **Problema del Oráculo**: Entiende por qué los smart contracts necesitan oráculos.
2. **Chainlink**:
   - [Documentación de Chainlink](https://docs.chain.link/)
   - [Chainlink Data Feeds](https://docs.chain.link/data-feeds)
   - [Chainlink VRF](https://docs.chain.link/vrf) para aleatoriedad verificable
   - [Chainlink Automation](https://docs.chain.link/chainlink-automation) para tareas programadas
3. **Proyectos Prácticos**:
   - Implementa un contrato que use feeds de precios
   - Crea una aplicación con aleatoriedad verificable
   - Automatiza la ejecución de funciones en tus contratos

### Cross-Chain y Bridges (CCIP)

1. **Interoperabilidad Blockchain**:
   - Comprende los desafíos de comunicación entre blockchains
   - Estudia los diferentes modelos de puentes (bridges)
2. **Chainlink CCIP (Cross-Chain Interoperability Protocol)**:
   - [Documentación de CCIP](https://docs.chain.link/ccip)
   - [Tutoriales de implementación](https://docs.chain.link/ccip/tutorials)
3. **Seguridad en Bridges**:
   - Estudia casos de hacks en bridges (Wormhole, Ronin, etc.)
   - Mejores prácticas de seguridad
4. **Proyectos Prácticos**:
   - Implementa un token que pueda moverse entre redes
   - Crea una aplicación que lea datos de múltiples blockchains
   - Desarrolla un sistema de mensajería cross-chain

## Agenda

Talleres ("office hours") de **lunes a viernes** en Discord. Se trabajará los proyectos de los cursos de Cyfrin Updraft, con Solidty o Vyper respectivamente.

Clases magistrales ("lectures") los **sábados** en Discord. Se explicará temas fundamentales de blockchain aplicados a smart contracts y los proyectos a desarrollar.

Se hará seguimiento semanalmente tanto al avance en los cursos (indiviualmente) como al desarrollo de los proyectos (grupalmente).

**¡No duden preguntar lo que sea en Discord o WhatsApp!**

## Referencia

[Documentación de Ethereum](https://ethereum.org/en/developers/docs/)

[Documentación de Base](https://docs.base.org/)

[Documentación de Polygon](https://docs.polygon.technology/)

[Documentación de Chainlink](https://docs.chain.link/)

[Documentación de Solidity](https://docs.soliditylang.org/en/latest/)

[Documentación de Foundry](https://book.getfoundry.sh/)

[Documentación de Vyper](https://docs.vyperlang.org/en/latest/)

[Documentación de Moccasin](https://cyfrin.github.io/moccasin/)

[Documentación de Nouns Builder](https://builder-docs.vercel.app/)

[Cyfrin Updraft](https://updraft.cyfrin.io/)

[CryptoZombies](https://cryptozombies.io/)

## Casos de estudio

### DAOs

- Nouns DAO
- **The Panama DAO**
- Developer DAO
- MakerDAO/Sky Protocol
- Aave

### Data

- The Graph
- Ocean Protocol
- ASI Alliance

## Proyectos

### `[SOLIDITY]` Nounish Gamified Freelancer DAO Marketplace

### `[VYPER]` Freelance Marketplace + Data Analysis Notebooks
