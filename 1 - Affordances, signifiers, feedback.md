# Análise: Componente de Aspeto / Seleção de Tema (YouTube)

Neste trabalho decidi fazer a análise do componente de seleção de aspeto e tema no YouTube, como demonstrado nas imagens abaixo:

<div align="center">

### Estados do Componente

| Tema do Dispositivo | Tema Escuro | Tema Claro |
| :---: | :---: | :---: |
| <img width="294" height="253" alt="Screenshot 2026-10-09 020134" src="https://github.com/user-attachments/assets/7151f1bc-7c19-46dd-b897-64cc81f79d0d" /> | <img width="295" height="254" alt="Screenshot 2026-10-09 020448" src="https://github.com/user-attachments/assets/c5db3f7a-c6c0-4a36-b2b6-3ea075b67f23" /> | <img width="293" height="252" alt="Screenshot 2026-10-09 020505" src="https://github.com/user-attachments/assets/a00fe1f7-1685-41b3-8d9f-f2b1b0fe2e66" /> |

</div>

---

## Questões da Interface

### Que ações é que o elemento permite de facto?
Permite ao utilizador definir a apresentação visual do YouTube no navegador através de três escolhas: sincronizar com as definições globais do sistema operativo ("Usar tema do dispositivo"), forçar a exibição do "Tema escuro" ou forçar a exibição do "Tema claro".

---

### Que ações parece permitir (affordances)?
Apresenta-se como uma lista vertical com texto legível. Pela natureza dos menus em interfaces digitais, sugere que cada linha é uma área clicável/interativa para seleção única, além do botão de seta à esquerda que sugere a ação de recuar ao menu anterior.

---

### Que signifiers existem?
* **Ícone de verificação (check mark):** Indica de forma clara qual é o item atualmente ativo na lista.
* **Cursor e efeito visual de foco/hover:** Ao passar o rato por cima de qualquer uma das três opções, o fundo da linha altera ligeiramente de cor, sinalizando que toda a linha é interativa e clicável.
* **Seta de navegação superior:** O ícone "←" junto à palavra "Aspeto" sinaliza visualmente a capacidade de retroceder na hierarquia do menu.
* **Mensagem informativa:** O texto secundário *"Esta definição aplica-se apenas a este navegador"* clarifica o âmbito da ação, informando que não afetará outros dispositivos.

---

### Algum signifier contraria a forma?
Sim. A lista não utiliza botões de rádio clássicos (os círculos com um ponto central habituais em seleções exclusivas). Em vez disso, usa apenas linhas de texto puro e um pisco. Isso pode inicialmente criar a dúvida se se trata de uma lista de ações imediatas ou de um menu de seleção contínua de opções.

---

### Que feedback devolve, e quando?
* **No elemento:** No momento do clique, o ícone de visto desloca-se instantaneamente para a linha clicada.
* **Global e imediato:** Toda a página do YouTube inverte imediatamente o esquema de cores (passa para fundo preto ou branco), permitindo verificar o resultado no mesmo segundo, sem necessidade de guardar ou recarregar.

---

### O que acontece quando existe alguma falha?
* **Navegador sem persistência (modo anónimo ou cookies bloqueados):** O tema muda no momento da seleção, mas assim que o separador é fechado a preferência perde-se, regressando ao padrão do dispositivo na sessão seguinte sem qualquer aviso de erro.
* **Falha de sincronização:** Ao escolher "Usar tema do dispositivo", se o sistema operativo não reportar corretamente a preferência de cor ao navegador, a interface pode assumir um tema padrão incorreto.

---

### Funciona sem visão ou sem rato?
* **Sem rato (teclado):** Sim. O menu pode ser percorrido usando a tecla `Tab` para entrar na lista e as setas direcionais (`↑` e `↓`) ou `Tab` para alternar entre as três opções, confirmando a escolha com a tecla `Enter` ou `Espaço`. A tecla `Esc` fecha o menu.
* **Sem visão (leitor de ecrã):** Sim. O componente é anunciado como um grupo de opções de rádio (`role="menuitemradio"`). O leitor de ecrã (como NVDA ou VoiceOver) lê o nome da opção e o seu estado (por exemplo: *"Usar tema do dispositivo, marcado"* ou *"Tema escuro, desmarcado"*), permitindo ao utilizador escolher sem depender de pistas visuais.
