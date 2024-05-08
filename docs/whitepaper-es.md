# Whitepaper Español Token Scol (Scolcoin) Smart Contracts

## Binance Smart Chain (BSC)

Nuestro contrato inteligente es BEP-20. Para obtener detalles técnicos sobre el estándar BEP-20: https://academy.binance.com/en/glossary/bep-20

Scolcoin (SCOL) token Nativo desarrollado en Solidity. Asegúrese de consultar su tutorial: https://solidity.readthedocs.io/en/v0.6.9/introduction-to-smart-contracts.html

Implementaciones de estándares ERC20

Source code: https://github.com/scolcoin/Token-Scolcoin-SCOL/blob/main/scolcoin.sol

## OpenZeppelin - Implementación segura

Nuestros Smart Contracts se basan en seguros y confiables [OpenZeppelin ERC-20 Smart Contract](https://docs.openzeppelin.com/contracts/4.x/erc20)

OpenZeppelin el código está en el corazón de nuestros tokens y seguimos sus prácticas de seguridad e implementación con mucho cuidado.

# Token Scolcoin (SCOL) 

Este token es una implementación estándar de ERC-20 y se implementó en la red principal de Binance Smart Chain con un suministro máximo fijo de 80,000,000 SCOL. Creacion de 1 SCOL tokens. Para arrancar el ecosistema Scolcoin Native Blockchain.

Mainnet Deployed Scolcoin (SCOL) Token can be found here: [https://bscscan.com/token/0x703477125bbee6430b2c4968c1ef66701a01359f](https://bscscan.com/address/0x069deca261ab51515c7b9af73c26c4ca339b6820)

Parámetros de compilación: Solidity 0.8.10+commit.fc410830. Optimización 200

## Proyecto Scolcoin
Nuestro proyecto nació el 3 de enero de 2018 con el bloque génesis de la cadena de bloques nativa Scolcoin (SCOL) que actualmente funciona en paralelo a nuestro token. Evolucionó con el protocolo POA donde nació el token Nativo con el contrato en nuestra red https://explorer.scolcoin.com/token/0xf25bFda0E59E9f946eA85Df4B9D52d298a3a7E81/

* Link Whitepaper 2.0.0.2 Scolcoin Nativo Blockchain
https://github.com/scolcoin/Whitepaper/blob/main/White%20Paper%20Scolcoin%20ver%202.0.0.2.pdf

## Criptomoneda SCOLCOIN (SCOL) Blockchain Nativa 2018 - 2022
El Proyecto Social Scolcoin en su etapa de creación fue presentado a la comunidad como el activo digital ecológico colombiano para alcanzar la fase Proof of Stake, logrando posicionamiento y reconocimiento en LatAm. Su bloque de génesis se realizó el 3 de enero de 2018, se conformaron los comités y presencia en comunidades.

* Link Código Scolcoin blockchain
https://github.com/scolcoin/scolcoin

* Scolcoin Blockchain Explorer
https://explorer.scolcoin.com/

## Característica Scolcoin 2018
* Name Scolcoin
* Abbreviation SCOL
* algorithm: Scrypt
* Type: PoW/PoS
* Letter Direction: S and T
* RPC port 51621
* P2P port 51622
* Block reward (POW) 1 coins
* Block reward (POS) 1 coins
* Total coin supply: 80,000,000 coins
* Last PoW block: block 10000
* Min. stake age 8 hours
* Max. stake age Unlimited
* Coinbase maturity 20 ( + 1 default confirmation) blocks
* Target spacing 5 minutes
* Target timespan 10 minutes
* Transaction confirmations 6 ( + 1 default confirmation) blocks

## Token Scolcoin (2024)
Desarrollado como un token en la red de Binance para lograr un puente entre las dos chains.

Basado en la wallet 0x8FCd63a667F0552c53aA45a1646b0Baade0eEc4b link explorador: https://bscscan.com/address/0x069deca261ab51515c7b9af73c26c4ca339b6820

// contracts/BEP20.sol
Source Code: https://github.com/scolcoin/Token-Scolcoin-SCOL
Link Contract: https://bscscan.com/address/0x069deca261ab51515c7b9af73c26c4ca339b6820#code

* /// @custom:security-contact info@scolcoin.com
* /***********************************************************
* Scolcoin (SCOL) cryptocurrency backup and investment toke
* ************************************************************/  
* // Copyright (c) 2018-2023 Scolcoin (SCOL) Native Blockchain
* // Copyright (c) 2024 Scolcoin (SCOL) token Native

## Desarrollo:

# 1 Fase:
Implementación del sistema Oraculo Scolcoin (blockchain).

# 2 Fase:
La implementación del sistema de conversión (Swap) se realizará mediante una API diseñada para la comunidad Scolcoin diseñada para intercambiar todas las monedas por token mediante la realización de una multiblockchain.

# 3 Fase:
Integración del proyecto PAD con el sistema multiblockchain API de Scolcoin. El proyecto PAD contiene un motor basado en inteligencia artificial para generar contratos inteligentes sobre una maquina virtual Scolcoin, con backup en redes publicas como soporte.

# Definición Oraculo Blockchain:
Portal estadístico de las cadenas blockchain actualmente propiedad del proyecto SCOL.

## Conversión:
la distribucion se realiza con la siguiente formula:
* Scolcoin Token Nativo en la red de Scolcoin wei Chain
* Scolcoin Token BSC.

Cambio 1 SCOL <> 1 SCOL

## Roadmap

# Q1 2021
* Noviembre de 2021: creación de Token Scolcoin (documento técnico, ANN, Exchange)

# Q2 2021
* Diciembre de 2021 - Lanzamiento del Fondo Pool Minero y Fondo de Liquidez.
* Inicio pool Minado. 
* Inicio pool Loquidez.
* (1 phase: Duración 2 Años)

# Q1 2022
* Enero a diciembre - Venta de activos a través de corredores de bolsa y / o corredores.
* Pago de recompensas del pool de minería (período mensual)

# Q1 2023
* Enero - Desarrollo de la plataforma Oracle (2 fases).

# Q2 2023
* Junio - Desarrollo de la plataforma del proyecto PAD (3 fases).

# Q1 2024
* Enero - Pool de minería de tiempo de retirada (1 fase).

# Q1 2025
* Enero - Lanzamiento del proyecto PAD (3 fases).

## Bibliotecas e interfaces

```Solidity
pragma solidity ^0.8.2;
```
Nosotros hemos desplegado Scolcoin token to mainnet with solidity ^0.8.2.

```Solidity
import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
```
De inmediato nos adentramos en el uso intensivo de las bibliotecas seguras de OpenZeppelin. Esta es la implementación básica de ERC-20 en la que se basa SCOL.

```Solidity
import "@openzeppelin/contracts/token/ERC20/extensions/ERC20Burnable.sol";
import "@openzeppelin/contracts/token/ERC20/extensions/ERC20Snapshot.sol";
import "@openzeppelin/contracts/access/AccessControl.sol";
import "@openzeppelin/contracts/security/Pausable.sol";
import "@openzeppelin/contracts/token/ERC20/extensions/draft-ERC20Permit.sol";
```
Ya hemos incluido scolcoin.sol, ¿por qué incluir la interfaz? El contrato inteligente de SCOL acepta un _token como uno de los parámetros de construcción. Discutiremos esto en la sección ** constructor ** a continuación.


## Exchange

* SCOL / USDT 


### ANN
https://bitcointalk.org/index.php?topic=5373860.msg58569225
