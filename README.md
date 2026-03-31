# Blacklist-Contract
Blacklist Contract
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Blacklist {
    mapping(address => bool) public banned;

    function ban(address user) public {
        banned[user] = true;
    }
}
