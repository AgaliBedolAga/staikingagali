require(addressStaked[_msgSender()] == false, “You already participated”); 

require(aplToken.balanceOf(_msgSender()) >= stakeAmount, “Insufficient Balance”);

aplToken.transferFrom(_msgSender(), address(this), stakeAmount);

stakeInfos[_msgSender()] = StakeInfo({      
      startTS: block.timestamp,          
      endTS: block.timestamp + planDuration,            
     amount: stakeAmount,                   
     claimed: 0 });

emit Staked(_msgSender(), stakeAmount);
