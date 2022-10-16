# communiti bootcamp assignment 1 
Create a smart contract which
Can take the name, and age while deploying the smart contract
A function that when called returns a name ;
A function that will only be accessible outside the smart contract and can return your age*2
Deploy your smart contract with Remix and test it


My solution

// SPDX-License-Identifier:MIT

pragma solidity 0.8.10;

contract Hi {
    string name;
    uint8 age;

	constructor(string memory _name, uint8 _age)  {
		name = _name;
         age =_age;
	}

	function getName() external view returns(string memory) {
		return name;
	}

	function setName(string memory _name) external {
		name = _name;
	}
     function getAge() external view returns(uint8) {
	 	return age*2;
	 }

	 function setAge(uint8 _age) external {
	 	age = _age;
	}
}


Note to myself: please pass name and age in constructor deploy button in remix when deploying.
