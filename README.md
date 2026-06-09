# snake
snakes wise
import time

def jornada_do_coelho():
    # Posições iniciais (em metros ou passos)
    posicao_coelho = 0
    posicao_cenoura = 5
    
    print("🐇 O coelho acordou e avistou uma cenoura deliciosa! 🥕")
    print(f"A cenoura está a {posicao_cenoura} passos de distância.\n")
    time.sleep(1)
    
    # Loop até o coelho alcançar a cenoura
    while posicao_coelho < posicao_cenoura:
        posicao_coelho += 1
        distancia_restante = posicao_cenoura - posicao_coelho
        
        print(f"Boing! O coelho deu um pulo. Posição atual: {posicao_coelho}")
        
        if distancia_restante > 0:
            print(f"Faltam {distancia_restante} passos...")
        else:
            print("O coelho chegou à cenoura!")
        
        time.sleep(0.8) # Pausa para dar efeito de animação no terminal
        print("-" * 30)

    print("\n🥕 Nhac! O coelho está feliz da vida comendo sua cenoura! 🐇🎉")

# Executar o código
jornada_do_coelho()
