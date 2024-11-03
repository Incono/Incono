
import time

# Simulation d'une liste de joueurs
players = {
    "player1": {"is_hacker": False},
    "hacker1": {"is_hacker": True},
    "player2": {"is_hacker": False},
}

def detect_hacker():
    for player, info in players.items():
        if info["is_hacker"]:
            ban_player(player)

def ban_player(player):
    print(f"Bannir le joueur: {player}")
    # Code pour bannir le joueur via l'API du jeu
    # Par exemple : api.ban(player)

# Boucle principale pour détecter les hackers
while True:
    detect_hacker()
    time.sleep(60)  # Vérifier toutes les minutes
