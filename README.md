# INTERNET
## DESCRIPTION

```mermaid

graph LR;
  C -->|One| D[Laptop]
  C -->|Two| E[iPhone]
  C -->|Three| F[fa:fa-car Car]
  D -->LB;
  E -->LB;
  F -->LB;  

LB-->nginx-01; 
LB-->nginx-02;
LB-->nginx-03;
nginx-01-->sqlserver;
nginx-02-->sqlserver;
nginx-03-->sqlserver;
sqlserver-->storage;
storage-->H
  H -->|One2| J[Laptop]
  H -->|Two2| L[iPhone]
  H -->|Three2| M[fa:fa-car Car]
```
