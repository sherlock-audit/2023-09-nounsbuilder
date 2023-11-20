
# Nouns Builder contest details

- Join [Sherlock Discord](https://discord.gg/MABEWyASkp)
- Submit findings using the issue page in your private contest repo (label issues as med or high)
- [Read for more details](https://docs.sherlock.xyz/audits/watsons)

# Q&A

### Q: On what chains are the smart contracts going to be deployed?
mainnet, Optimism, Base, Zora
___

### Q: Which ERC20 tokens do you expect will interact with the smart contracts? 
none
___

### Q: Which ERC721 tokens do you expect will interact with the smart contracts? 
no external tokens
___

### Q: Which ERC777 tokens do you expect will interact with the smart contracts? 
none
___

### Q: Are there any FEE-ON-TRANSFER tokens interacting with the smart contracts?

none
___

### Q: Are there any REBASING tokens interacting with the smart contracts?

none
___

### Q: Are the admins of the protocols your contracts integrate with (if any) TRUSTED or RESTRICTED?
TRUSTED
___

### Q: Is the admin/owner of the protocol/contracts TRUSTED or RESTRICTED?
TRUSTED
___

### Q: Are there any additional protocol roles? If yes, please explain in detail:
none
___

### Q: Is the code/contract expected to comply with any EIPs? Are there specific assumptions around adhering to those EIPs that Watsons should be aware of?
none
___

### Q: Please list any known issues/acceptable risks that should not result in a valid finding.
When calling L2MigrationDeployer.deploy the L2MigrationDeployer address must be set as the first founder in the founders array or the call will revert
___

### Q: Please provide links to previous audits (if any).
https://code4rena.com/reports/2022-09-nouns-builder
___

### Q: Are there any off-chain mechanisms or off-chain procedures for the protocol (keeper bots, input validation expectations, etc)?
L2MigrationDeployer transactions can reach above the max purchased gas for L1CrossDomainMessenger relayMessage calls. These transactions will be resubmitted by our relayer.
___

### Q: In case of external protocol integrations, are the risks of external contracts pausing or executing an emergency withdrawal acceptable? If not, Watsons will submit issues related to these situations that can harm your protocol's functionality.
yes
___

### Q: Do you expect to use any of the following tokens with non-standard behaviour with the smart contracts?
none
___

### Q: Add links to relevant protocol resources
https://hackmd.io/peXISQ2CSQOwRGmvpUpK9A?view
___




# Audit scope