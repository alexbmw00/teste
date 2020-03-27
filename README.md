# INTERNET
## DESCRIPTION

```mermaid

graph LR;
  LINK -->|One| C1[Laptop]
  LINK -->|Two| C2[iPhone]
  LINK -->|Three| C3[Desktop]
  C1 -->LB;
  C2 -->LB;
  C3 -->LB;  

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
