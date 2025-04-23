<script type="text/javascript">
    var num, bin = "";
    var dec = 0;

    // Solicita entrada do usuário
    num = parseInt(window.prompt("Digite um número inteiro positivo:"));

    if (num >= 0) {
        if (num === 0) {
            bin = "0"; // Caso especial para o número 0
        } else {
            while (num > 0) {
                if (num % 2 === 0) {
                    bin = "0" + bin;
                } else {
                    bin = "1" + bin;
                }
                num = Math.floor(num / 2);
            }
        }
        document.write("O número em binário é: " + bin);
    } else {
        document.write("Por favor, digite um número positivo.");
    }
</script>
