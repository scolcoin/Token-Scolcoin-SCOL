# Whitepaper Token Scol (Scolcoin) 2.0 Our Smart Contracts

## Binance Smart Chain (BSC)

Our smart Contracts are BEP-20. For Techincal Details on BEP-20 Standard: https://academy.binance.com/en/glossary/bep-20

Scolcoin (SCOL) tokens were written in Solidity. Be sure to check out their tutorial before jumping into code: https://solidity.readthedocs.io/en/v0.6.9/introduction-to-smart-contracts.html

Implementations of standards ERC20

Source code: https://github.com/scolcoin/Token-Scolcoin-SCOL/blob/main/scolcoin.sol

## OpenZeppelin - The secure implementation

Our Smart Contracts are based on secure and trusted [OpenZeppelin ERC-20 Smart Contract](https://docs.openzeppelin.com/contracts/4.x/erc20)

OpenZeppelin code is at the heart of our tokens and we follow their security practices and implementation very carefully.

# Scolcoin (SCOL) Token

This token is a standard ERC-20 implementation and was deployed on Binance Smart Chain mainnet with fixed Max Supply of 80,000,000 SCOL. 1 SCOL tokens were ultimately. To bootstrap the Scolcoin Native Blockchain ecosystem.

Mainnet Deployed Scolcoin (SCOL) Token can be found here: https://bscscan.com/token/0x703477125bbee6430b2c4968c1ef66701a01359f

Compilation Parameters: Solidity 0.8.10+commit.fc410830. Optimization 200

## Libraries & Interfaces

```Solidity
pragma solidity ^0.8.2;
```
We've deployed Scolcoin token to mainnet with solidity ^0.8.2.

```Solidity
import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
```
Right away we get into the heavy usage of OpenZeppelin secure libraries. This is the base ERC-20 implementation that SCOL is based on.

```Solidity
import "@openzeppelin/contracts/token/ERC20/extensions/ERC20Burnable.sol";
import "@openzeppelin/contracts/token/ERC20/extensions/ERC20Snapshot.sol";
```
We've already included scolcoin.sol, why include the interface? SCOL smart contract accepts a _token as one of the constructore parameters. We'll discuss this in the **constructor** section below.

## ERC20Burnable
Our Token can perform the function of Burning Token, make Repurchases to be able to Burn Tokens
** _burn(account, amount); **

Code:
/**
 * @dev Extension of {ERC20} that allows token holders to destroy both their own
 * tokens and those that they have an allowance for, in a way that can be
 * recognized off-chain (via event analysis).
 */
abstract contract ERC20Burnable is Context, ERC20 {
    /**
     * @dev Destroys `amount` tokens from the caller.
     *
     * See {ERC20-_burn}.
     */
    function burn(uint256 amount) public virtual {
        _burn(_msgSender(), amount);
    }

    /**
     * @dev Destroys `amount` tokens from `account`, deducting from the caller's
     * allowance.
     *
     * See {ERC20-_burn} and {ERC20-allowance}.
     *
     * Requirements:
     *
     * - the caller must have allowance for ``accounts``'s tokens of at least
     * `amount`.
     */
    function burnFrom(address account, uint256 amount) public virtual {
        uint256 currentAllowance = allowance(account, _msgSender());
        require(currentAllowance >= amount, "ERC20: burn amount exceeds allowance");
        unchecked {
            _approve(account, _msgSender(), currentAllowance - amount);
        }
        _burn(account, amount);
    }
}

// File: contracts/scolcoin.sol

// contracts/BEP20.sol

