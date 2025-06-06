# Documentação Tailwind

**-> Instalando a versão 3 do Tailwind:** npm install -D tailwindcss@3.3.5
**-> Inicializando o Tailwind:** npx tailwindcss init -p
[🔗 Tailwind](https://v2.tailwindcss.com/)

**-> Instalando componentes usando Shadcn:** npx shadcn@latest add button
[🔗 Shadcn](https://ui.shadcn.com/)

**-> Flowbite componentes prontos:** https://flowbite.com/docs/components/card/ 

# Propriedades do Css no Tailwind

* Flexbox: flex justify-center items-center

* Grid: grid place-items-center

* Horizontal apenas: mx-auto

* Bordas: border, border-color-intensidade, rounded (Cantos redondos)

* W: Width, H: Height. (-Full, pega a largura total do contêiner)

* M: Margin, se for colocar para alguma direção específica, só acrescentar a primeira letra do lado. Ex: mt(Margin-top)
  A mesma com o P.

* Sombras: Shadow

* Imagem BackGround: bg-[url('/caminho/da/imagem.jpg')], bg-no-repeat

* Elemento Flutuar: Float, para cancelar usa o clear-both

* Posição: relative, absolute, fixed

* Fonte e Texto: Text-, font-nomedafonte, font-bolt e font-light, text-direçãoParaAlinhamento

* Espaçamento entre itens: Gap

* opacidade: opacity-intensidade

* Transição: trasition, duration, hover

# Responsividade

| Prefixo | Largura mínima (px) | Exemplo de dispositivo                  |
| ------- | ------------------- | --------------------------------------- |
| `sm:`   | 640px               | Smartphones grandes, tablets em retrato |
| `md:`   | 768px               | Tablets em paisagem ou laptops pequenos |
| `lg:`   | 1024px              | Laptops e desktops padrão               |
| `xl:`   | 1280px              | Monitores grandes                       |
| `2xl:`  | 1536px              | Telas ultra-grandes                     |

| Exemplo 
|-------------------------------------------------|
|"text-sm md:text-base lg:text-lg" -> Texto que aumenta de tamanho conforme a tela!      |

* flex-col -> Para telas menores, os elementos ficam empilhados verticalmente.
* flex-row -> Elementos lado a lado

# Hidden

**-> hidden md:flex** Esconde em telas pequenas, flex em telas médias

**-> hidden md:block** Esconde em telas pequenas

**-> block md:hidden** Aparece em telas pequenas

**-> overflow-hidden:** Oculta tudo que passar do contêiner.

# Alinhamentos

 **class="absolute top-0 right-0" ->** Esse se refere a objeto no canto superior direito, contudo, se for inferior só mudar para bottom. </br>
 Se for esquerdo só colocar left. 

 * w-1/2 junto com flex-1 no que deseja dividir

 # Rolagem

* overflow-auto – cria uma barra de rolagem quando necessário
* overflow-scroll – sempre mostra a barra de rolagem
* overflow-hidden – oculta tudo que ultrapassar
* overflow-x-auto – rolagem só horizontal
* overflow-y-auto – rolagem só vertical

# Colunas

| Exemplo 
|-------------------------------------------------|
|grid grid-cols-3 gap-4 | grid-cols-3: 3 colunas && gap-4: espaçamento entre itens   |

# Estilizações

bg-*: cor de fundo.
bg-gradient-to-*: gradiente em direção a (r, l, t, b).
from-*, to-*: cores do gradiente.
Exemplo: bg-gradient-to-r from-blue-500 to-purple-500

blur -> backdrop-bur-intensidade
Backdrop: Fundo

# Arquivos

**-> App.css ou algum CSS principal:**

@tailwind base;
@tailwind components;
@tailwind utilities;

