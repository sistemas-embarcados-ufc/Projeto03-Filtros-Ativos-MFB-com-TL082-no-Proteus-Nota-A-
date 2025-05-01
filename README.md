# 🎚️ Projeto03 – Filtros Ativos MFB com TL082 no Proteus (Nota A)

Este projeto simula dois filtros ativos de segunda ordem com topologia MFB (Multiple Feedback), utilizando o amplificador operacional TL082 no Proteus. O objetivo é analisar como filtros passa-alta e passa-baixa afetam o timbre da nota musical A (440 Hz), tanto visualmente (via osciloscópio e gráfico de frequência) quanto auditivamente (via speaker).

---

## 🎛️ Esquema do Circuito

<p align="center">
  <img src="Imagens/esquema_projeto03.png" width="600px">
</p>

### 🔧 Configuração:

- **Tipo de filtro**: MFB Ativo (2ª ordem)
- **CI utilizado**: TL082
- **Fonte**: Simétrica (±12V)
- **Entrada de sinal**: Nota musical A (senoidal de 440 Hz)
- **Saída**:
  - Conectada ao osciloscópio
  - Conectada ao gráfico de análise de frequência
  - Conectada ao speaker

---

### 🔊 Filtro Passa-Alta

- **Objetivo**: Eliminar frequências graves abaixo da nota A.
- **Frequência de corte (fc)**: ~100 Hz
- **Componentes utilizados**:
  - C1 = C2 = C3 = 160 nF
  - R1 = R2 = 10kΩ

---

### 🔉 Filtro Passa-Baixa

- **Objetivo**: Atenuar frequências acima da nota A.
- **Frequência de corte (fc)**: ~350 Hz
- **Componentes utilizados**:
  - R1 = R2 = R3 = 5.6kΩ
  - C1 = C2 = 82 nF

---

## 🧰 Como Simular no Proteus

1. Abra o arquivo .pdsprj no Proteus.
2. Pressione ▶️ para iniciar a simulação.
3. Observe os sinais no osciloscópio:
   - CH A: sinal puro da nota A (entrada)
   - CH B: sinal filtrado (saída)
4. Use o analisador de frequência para visualizar a resposta espectral dos filtros.
5. Ouça a diferença no timbre usando o speaker:
   - O passa-alta deixa o som mais estridente/brilhante.
   - O passa-baixa deixa o som mais abafado/suave.

---

## 📈 Análise do Resultado

<p align="center">
  <img src="Imagens/frequencia_projeto03.png" width="600px">
</p>

- O filtro passa-alta remove os graves e realça os harmônicos da nota A, podendo até lembrar uma onda mais quadrada se houver conteúdo harmônico.
- O filtro passa-baixa elimina os agudos e suaviza o som da nota A, reduzindo brilho e presença.

---

## 💡 Observações

- A escolha da nota A (440 Hz) permite observar como cada filtro atua sobre frequências musicais comuns.
- A topologia MFB garante estabilidade e uma boa curva de resposta para filtros de segunda ordem.
- O TL082 é um amplificador operacional adequado para aplicações de áudio em simulação, com boa largura de banda para as frequências analisadas.
