# Do Zero ao Império Industrial 3D

Versão 3D para navegador, feita com HTML5, CSS3, JavaScript e **Three.js**.
O jogador começa com **R$ 100** e uma bancada manual numa fábrica de caixas de papelão e precisa transformá-la numa indústria totalmente automatizada.

## Como jogar

Dê dois cliques no `index.html`. Ele abre no Chrome, Edge ou Firefox, sem instalar nada e **sem precisar de internet**, porque o Three.js já está na pasta `js/`.

| Tecla | Ação |
|---|---|
| WASD ou setas | Andar |
| E ou Espaço | Interagir (segure na bancada para montar) |
| L ou Tab | Abrir/fechar a loja |
| Esc ou P | Pausar |

## Processo de fabricação

1. **Comprar**: no balcão do fornecedor (10 papelões = R$ 20).
2. **Transportar**: pegar o papelão no palete e levar até a bancada ou máquina.
3. **Fabricar**: segurar E na bancada (as máquinas trabalham sozinhas).
4. **Armazenar**: levar as caixas prontas até o estoque.
5. **Entregar**: vender na expedição (R$ 5 por caixa, R$ 7 em pedidos).

## Progressão

| Nível | Desbloqueio |
|---|---|
| 1. Produção manual | Bancada, palete, estoque e expedição |
| 2. Primeiros equipamentos | Estilete, carrinho, bancada profissional e dobradeira (R$ 250) |
| 3. Funcionários | Funcionários (R$ 500) que transportam, montam e organizam o estoque |
| 4. Automatização | Esteira, contrato com fornecedor, transportadora e montadora automática |
| 5. Grande indústria | Expansão do galpão e automação total (vitória) |

## Organização do código

| Arquivo | Função |
|---|---|
| `js/jogo.js` | Estado, economia, produção, loja, missões e salvamento |
| `js/cena.js` | Fábrica 3D, máquinas, esteira, caminhão e textos sobre a cena |
| `js/personagens.js` | Jogador (movimento e colisão) e inteligência dos funcionários |
| `js/interface.js` | HUD, loja, menus, mensagens e sons |
| `js/principal.js` | Teclado, tecla E e laço principal |
| `js/three.min.js` | Biblioteca Three.js r128 |

Para equilibrar o jogo, mude as constantes da seção **ECONOMIA** no início de `js/jogo.js`.
O progresso fica salvo no próprio navegador (localStorage).
