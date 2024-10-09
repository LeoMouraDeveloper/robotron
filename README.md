# robotron-2000

function atualizaEstatisticas(operacao, peca) {

    estatisticas.forEach( (elemento) => {
        if (operacao === "+") {
            elemento.textContent = parseInt(elemento.textContent) + pecas[peca][elemento.dataset.estatistica]
        }else{
            elemento.textContent = parseInt(elemento.textContent) - pecas[peca][elemento.dataset.estatistica]
        }
       
    })
}
