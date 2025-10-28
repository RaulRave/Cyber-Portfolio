# Semana 1 – Día 1: Bandit niveles 0–3
## 🔐 Objetivo
Practicar comandos básicos de Linux y resolver niveles iniciales de OverTheWire Bandit.

# Semana 1 – Día 1: Bandit niveles 0–3

## 🔐 Objetivo
Practicar comandos básicos de Linux y resolver niveles iniciales de OverTheWire Bandit.

🧩 Paso a paso
    1. Conéctate a Bandit
       bash
       ssh bandit0@bandit.labs.overthewire.org -p 2220
       Contraseña: bandit0
       🧩 Nivel 0 → 1
🎯 Objetivo
Encontrar la contraseña del usuario bandit1 leyendo el archivo readme.
✅ Comando
bash
ls
→ Muestra los archivos del directorio actual. Verás readme.
bash
cat readme
→ Muestra el contenido del archivo. Esa es la contraseña para el siguiente nivel.
Congratulations on your first steps into the bandit game!!
Please make sure you have read the rules at https://overthewire.org/rules/
If you are following a course, workshop, walkthrough or other educational activity,
please inform the instructor about the rules as well and encourage them to
contribute to the OverTheWire community so we can keep these games free!

The password you are looking for is: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
📌 ¿Por qué se hace?
    • Aprendes a listar archivos (ls)
    • Lees contenido con cat
    • Empiezas a navegar por el sistema
✍️ Anota la contraseña para usarla en el siguiente nivel.
🧩 Nivel 1 → 2
🎯 Objetivo
Leer un archivo llamado -, que parece un parámetro.
✅ Comando
1. Sal de cualquier sesión activa
Si estás dentro de Bandit, escribe:
bash
exit
2. Conéctate al nivel 1 correctamente
bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
→ Cuando te pida la contraseña, escribe:
Código
ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

bash
cat ./-
→ Usamos ./- para indicar que es un archivo, no una opción de cat.
📌 ¿Por qué se hace?
    • Aprendes a manejar nombres de archivo conflictivos
    • Usas rutas relativas (./) para evitar errores
✍️ Anota la contraseña para el siguiente nivel.
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
🧩 Nivel 2 → 3
🎯 Objetivo
Leer un archivo con espacios en el nombre.
Sal del nivel 1 si aún estás dentro:
       bash
       exit
    1. Conéctate al nivel 2:
       bash
       ssh bandit2@bandit.labs.overthewire.org -p 2220
       → Usa esta contraseña:
       Código
       263JGJPfgU6LtdEvgfWU1XP5yac29mFx
    2. Una vez dentro, ejecuta:
       bash
       ls --spaces in this filename--
       cat -- "--spaces in this filename--"
       ✍️ Anota la contraseña para el siguiente nivel.
       MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
📌 ¿Por qué se hace?
    • Aprendes a manejar nombres con espacios
    • Usas comillas para evitar errores de parsing

🧩 Nivel 3 → 4
🎯 Objetivo
Leer un archivo oculto (comienza con .)
✅ Comando
Bash
Entra al directorio inhere:
bash
cd inhere
    • Lista los archivos ocultos:
bash
ls -la
...Hiding-From-You

cat "...Hiding-From-You"
→ Muestra la contraseña.
📌 ¿Por qué se hace?
    • Aprendes a listar archivos ocultos
    • Usas ls -la para ver permisos y propietarios
✍️ Anota la contraseña para el siguiente nivel.
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ



