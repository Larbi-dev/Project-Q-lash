# Project-Q-lash

Live multiplayer quiz tournament platform:
combining:
• Real-time competition
• Category voting
• Leaderboard + elimination rounds
• Fun, social, and educational

Let’s visualize the full game architecture and flow.

🎮Core Game Flow

1. 🏁Start Room / Lobby

• Players enter room with a unique code or join public game.
• Lobby screen shows all participants.
• Live vote: Pick quiz category (e.g., Science, Football, Politics).
• Highest voted category is locked in.
 Add chat in the lobby for social touch.
 
2. ⏳Countdown Phase
   
• 10-second timer shown to all players.
• Message: “Get Ready… Your quiz begins in 10 seconds!”
 Add sound effect and flashing animations.
 
4. 🧩Round 1: Quiz Battle Begins
   
• 15 multiple-choice questions
• Each shown for a fixed time (e.g. 15 seconds)
• Answer submitted → locked
• Show live progress bar (time remaining)
 Award points for:
• Correct answer
• Speed of response (faster = more points)

6. 🪓Cut-Off Phase: Elimination

• Pass mark set (e.g., 9/15 or 60%)
• Players below the line are eliminated
• Leaderboard shown to everyone
 "You’ve been eliminated" screen with stats
 Top performers advance

7. 🔁Next Round(s)

• New round begins with same structure
• Continue until only top 3 remain
• Final round: Speed round (5 quick-fire questions)
🏆6. Final Leaderboard + Celebration
• Crown the winner
• Medal animation for 2nd & 3rd place
• Option to replay or share score
 Winner gets a custom animated card (can download)
 Option to play again or start new room

📐Architecture Overview

Component Tech Stack Suggestion
Frontend HTML, CSS, JavaScript, React (for smooth UI)
Real-time Game
Logic
Socket.io (real-time updates)
Backend Node.js + Express (or Django/Flask if preferred)
Database MongoDB / Firebase / PostgreSQL
Quiz Data
JSON/DB (you can start with hardcoded
questions)
