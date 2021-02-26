# JMeter Tips

## Refs


## Gerar resultados em HTML Reports (APDEX)

jmeter -g <log file> -o <Path to output folder>
  
## Executar em linha de comando

## Melhore o desempenho dos scripts utilizando estas técnicas (Regras)

<ol>
  <li>Use o modo CLI.</li>
  <li>Use o mínimo de Listeners possível, se estiver usando o sinalizador -l na linha de comando, todos os Listeners podem ser excluídos ou desabilitados.</li>
  <li>Não use os ouvintes "View Results Tree" ou "View Results in Table" durante o teste de carga, use-os apenas durante a fase de script para depurar seus scripts.</li>
  <li>Em vez de usar muitos amostradores semelhantes, use o mesmo amostrador em um loop e use variáveis (Conjunto de dados CSV) para variar a amostra. [O controlador de inclusão não ajuda aqui, pois adiciona todos os elementos de teste do arquivo ao plano de teste.]</li>
  <li>Não use o modo funcional (Functional Mode).</li>
  <li>Use a saída CSV em vez de XML.</li>
  <li>Salve apenas os dados de que você precisa.</li>
  <li>Use o mínimo possível de Assertivas (Assertions).</li>
  <li>Use a linguagem de script de melhor desempenho (consulte a seção JSR223).</li>
</ol>
