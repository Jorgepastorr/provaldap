# provaldap



Imagen docker con servidor ldap dominio `dc=jorge,dc=cat` 



## Estructura

raiz  jorge.cat  organizacion socios con e socios con dn `ldcat=111,ou=socis,dc=jorge,dc=cat` consecutivamente ldcat 222, 333

## Funcionamiento

```bash
docker run --name ldapserver -h ldapserver -d jorgepastorr/provaldap
```



## extra

```bash
ldapadd -x -D cn=Manager,dc=jorge,dc=cat -w secret -f mod.ldif
```

no funciona conflicto de objeto


