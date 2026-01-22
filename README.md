# eth9
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleNFT {
    uint256 public tokenId;
    mapping(uint256 => address) public ownerOf;

    function mint() public {
        tokenId++;
        ownerOf[tokenId] = msg.sender;
    }
}
