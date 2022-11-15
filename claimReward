uint256 stakeAmount = stakeInfos[_msgSender()].amount; 

uint256 totalTokens = stakeAmount + (stakeAmount * interestRate / 100); 

stakeInfos[_msgSender()].claimed == totalTokens; 

aplToken.transfer(_msgSender(), totalTokens); 

emit Claimed(_msgSender(), totalTokens);
