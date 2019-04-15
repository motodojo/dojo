```
unordered_map<string, vector<string>> network {
    { "Min",     { "William", "Jayden", "Omar" } },
    { "William", { "Min", "Noam" } },
    { "Jayden",  { "Min", "Amelia", "Ren", "Noam" } },
    { "Ren",     { "Jayden", "Omar" } },
    { "Amelia",  { "Jayden", "Adam", "Miguel" } },
    { "Adam",    { "Amelia", "Miguel", "Sofia", "Lucas" } },
    { "Miguel",  { "Amelia", "Adam", "Liam", "Nathan" } },
    { "Noam",    { "Nathan", "Jayden", "William" } },
    { "Omar",    { "Ren", "Min", "Scott" } }
};
```
Given information about active users on the network, find the shortest route for a message from one user (the sender) to another (the recipient). 
Return a vector of users that make up this route. 

For the network above, a message from Jayden to Adam should have this route: 

```
{ "Jayden", "Amelia", "Adam" }
```
