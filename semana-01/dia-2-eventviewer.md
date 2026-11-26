# Día 2 — Análisis de Eventos de Autenticación en Windows

## Objetivo

Entender los eventos 4624 y 4625 del Windows Security Log y su relevancia para un analista de seguridad.


## Event ID 4624 — Inicio de sesión exitoso

- Qué significa: Son los inicios de sesión exitosos.
- Campos clave: Account Name, Logon Type 
- Ejemplo observado: [cuenta DESKTOP-1A6JVAD$, logon type 5]
- Por qué importa: Su importancia radica en que se pueden auditar y saber quién inicia sesión y desde dónde.

## Event ID 4625 — Inicio de sesión fallido

- Qué significa: Son los intentos de inicio de sesión fallidos. 
- Campos clave: Account Name, Logon Type, Failure Reason
- Ejemplo observado: [cuenta, DESKTOP-1A6JVAD$ logon type 2]
- Por qué importa:Podemos detectar cuando alguien intentó iniciar sesión.




## Tipos de Logon más comunes

- Type 2: Local
- Type 3: Red
- Type 10: RDP
- (otros que veas) 11, 7

## Conclusión

¿Qué aprendí hoy y cómo lo usaría en un SOC? Aprendí a auditar mi equipo si en algún momento dado alguien quiere utilizar mi equipo puedo detectarlo.