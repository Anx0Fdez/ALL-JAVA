# ***PostgreSQL***
### *by: [Anxo Fdez]*
#### *github: [Anx0Fdez](https://github.com/Anx0Fdez)*

---
### `PRO-TIPS`
*No se deben poner tildes ni caracteres especiales en los nombres de las tablas, columnas, codigo, etc.*

*No se permite el uso de `ñ` con el objetivo de evitar problemas de codificación.*

---

### *Iniciar terminal de PostgreSQL*
```bash
pslq postgres
```

### *Meter archivos sql en la terminal de PostgreSQL*
```bash
\i /path/to/file.sql
```

## *Estrucuturas básicas*
### `PROCEDIMIENTOS`
```postgresql
create or replace procedure /*ptimpidep*/(/*vnum_persoa varchar*/)
language plpgsql as $$

declare

begin

end;$$
```
#### <u>*Lanzamiento de Procedimientos*</u>
```postgresql
call /*ptimpidep*/(/*Jose*/);
```

### `TRIGGERS`
```postgresql
drop trigger if exists /*timpidep*/ on /*a1c*/;

create or replace function /*ftimpidep*/() returns trigger 
language plpgsql as $$

declare

begin

return new;
end;$$
;
create trigger /*timpidep*/ before insert on /*a1c*/ for each row execute procedure /*ftimpidep*/()
```
#### <u>*Lanzamiento de Triggers*</u>
```postgresql
insert into /*a1c*/ values (/*1, 2, 3, 4, 5, 6, 7, 8, 9, 10*/);
```

### `FUNCIONES`
```postgresql

```







