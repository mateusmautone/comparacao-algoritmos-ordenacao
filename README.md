# Comparação de Algoritmos de Ordenação 🔄

Este projeto realiza a comparação entre vários algoritmos de ordenação. Ele mede o tempo de execução, número de comparações e trocas para diferentes algoritmos. O projeto também coleta métricas de desempenho usando **Prometheus** e **OpenTelemetry**.

## Algoritmos Implementados ⚙️

O projeto inclui as seguintes implementações de algoritmos de ordenação:

- **Bubble Sort** 🟢
- **Bubble Sort Otimizado** 🟢
- **Insertion Sort** 🔵
- **Selection Sort** 🟡
- **Quick Sort** 🔴
- **Merge Sort** 🟣
- **Heap Sort** 🟤
- **Counting Sort** (comentado no código) 🟠
- **Radix Sort** (comentado no código) 🟣
- **Shell Sort** (comentado no código) ⚫

## Requisitos 📦

- Python 3.x 🐍
- Bibliotecas necessárias:
  - `werkzeug` ⚙️
  - `prometheus_client` 📊
  - `opentelemetry-sdk` 🔧
  - `flask` 🔥
  - `random` 🎲

Você pode instalar as dependências com o comando:

```bash
pip install -r requirements.txt
```

Isso irá testar os algoritmos de ordenação com listas de tamanhos 1.000 e 10.000 e exibir os resultados no terminal.

Monitoramento com Prometheus 📈
O projeto utiliza o Prometheus para coletar métricas de desempenho. Para isso, o arquivo metrics_server.py expõe uma rota /metrics, onde Prometheus pode coletar os dados.

Execute o servidor de métricas com:

`python metrics_server.py`

O servidor ficará disponível em http://localhost:7070/metrics, onde as métricas serão expostas.

Análise de Desempenho 📊
Ao rodar o código, você verá o tempo de execução, o número de comparações e o número de trocas realizadas por cada algoritmo. Isso pode ser útil para comparar a eficiência dos algoritmos com diferentes tamanhos de entrada.


## Conclusão 💡

Este projeto fornece uma comparação eficiente entre diversos algoritmos de ordenação, permitindo avaliar seu desempenho em termos de tempo de execução, comparações e trocas. Além disso, o monitoramento com **Prometheus** permite uma análise detalhada das métricas de execução, ajudando a entender como cada algoritmo se comporta com diferentes volumes de dados. Com isso, é possível escolher o algoritmo mais adequado para cada situação com base nos requisitos de desempenho.
