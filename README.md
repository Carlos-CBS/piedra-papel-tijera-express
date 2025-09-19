# ✂️ Piedra, Papel o Tijera - Multiplayer

## 📌 Descripción

Este proyecto es un juego de **Piedra, Papel o Tijera** para dos jugadores, desarrollado en JavaScript y ejecutado en **Node.js con Express**.  

Incluye dos modos de backend:

1. **REST**: con un frontend funcional en HTML + JS puro (sin estilos todavía). Toda la lógica se guarda en memoria (arrays de objetos).  
2. **GraphQL**: permite iniciar partidas, mover jugadores y consultar resultados mediante queries y mutations. Actualmente **no tiene frontend**, solo se puede usar desde GraphiQL o clientes GraphQL.

> ⚡ Todos los datos están en memoria, **no se utiliza ninguna base de datos externa**.

---

## 🚀 Funcionalidades principales

### REST + Frontend

- 🆕 Crear partidas nuevas  
- ✋ Elegir jugadas para **player1** y **player2**  
- 📊 Ver el conteo de victorias, derrotas y empates  
- 🔎 Consultar el estado actual de la partida  
- 🔄 Finalizar partidas  
- 💻 Frontend funcional en HTML + JavaScript puro

### GraphQL (sin frontend)

- 🆕 `iniciarJoc(codiPartida: Int!)` → crea una nueva partida  
- ✋ `moureJugador(codiPartida: Int!, jugador: Int!, tipusMovimiento: String!)` → registrar jugada de un jugador  
- 🔎 `consultarEstat(codiPartida: Int!)` → consultar el estado de la partida  
- ❌ `acabarJoc(codiPartida: Int!)` → eliminar la partida

---

## 🛠️ Tecnologías utilizadas

- **Node.js** (runtime)  
- **Express** (para el backend REST y servir frontend)  
- **HTML5 + JavaScript puro** (frontend funcional)  
- **express-graphql + graphql** (backend GraphQL)  
- Arrays y objetos en JS para almacenar partidas en memoria  

---

## 📥 Instalación y ejecución

1. Clonar el repositorio:

```bash
git clone https://github.com/tu-usuario/piedra-papel-tijera.git
cd piedra-papel-tijera
