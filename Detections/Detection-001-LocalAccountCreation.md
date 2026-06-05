Suspicious Local Account Creation

Behavior:

Creation of a local Windows account using net.exe

Evidence:

CommandLine:
net1 user cyberlab Password123! /add

User:
Mahi\buddh

Parent Process:
net.exe

Why It Matters:

Attackers may create local accounts to maintain access.

Investigation Questions:

Who created the account?
Was it expected?
Was there a change ticket?
Was the account added to Administrators?
