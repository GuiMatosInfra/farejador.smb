<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instalação do enum4linux no Debian</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        header {
            background: #333;
            color: #fff;
            padding-top: 30px;
            min-height: 70px;
            border-bottom: #bbb 1px solid;
        }
        header h1 {
            text-align: center;
            margin: 0;
        }
        code {
            background: #e9e9e9;
            padding: 2px 5px;
            border-radius: 3px;
        }
        .steps {
            background: #fff;
            padding: 20px;
            border: 1px solid #ddd;
            margin-bottom: 20px;
        }
        h2 {
            border-bottom: 2px solid #333;
            padding-bottom: 10px;
        }
        pre {
            background: #f4f4f4;
            padding: 10px;
            border: 1px solid #ddd;
            overflow-x: auto;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Instalação do enum4linux no Debian</h1>
        </div>
    </header>
    <div class="container">
        <section class="steps">
            <h2>Passos para Instalação</h2>
            <ol>
                <li>
                    <strong>Atualizar o Sistema</strong>
                    <pre><code>sudo apt update
sudo apt upgrade</code></pre>
                </li>
                <li>
                    <strong>Instalar Dependências</strong>
                    <pre><code>sudo apt install python python-pip git</code></pre>
                </li>
                <li>
                    <strong>Clonar o Repositório</strong>
                    <p>Dependendo do repositório específico, utilize um dos seguintes comandos:</p>
                    <ul>
                        <li><strong>Repositório da Cisco:</strong></li>
                        <pre><code>git clone https://github.com/cisco/enum4linux.git</code></pre>
                        <li><strong>Repositório da CXSecurity:</strong></li>
                        <pre><code>git clone https://github.com/cxsecurity/enum4linux.git</code></pre>
                    </ul>
                </li>
                <li>
                    <strong>Navegar para o Diretório</strong>
                    <pre><code>cd enum4linux</code></pre>
                </li>
                <li>
                    <strong>Tornar o Script Executável</strong>
                    <pre><code>chmod +x enum4linux.pl</code></pre>
                </li>
                <li>
                    <strong>Executar o enum4linux</strong>
                    <pre><code>./enum4linux.pl &lt;endereço_IP&gt;</code></pre>
                    Substitua <code>&lt;endereço_IP&gt;</code> pelo endereço IP do alvo que você deseja escanear.
                </li>
            </ol>
        </section>
        <section class="steps">
            <h2>Exemplo de Execução</h2>
            <pre><code>./enum4linux.pl -a 10.10.133.29</code></pre>
        </section>
        <section class="steps">
            <h2>Notas Importantes</h2>
            <p><strong>Permissões e Legislação:</strong> Sempre obtenha permissão antes de realizar qualquer varredura em redes ou sistemas. A execução não autorizada de ferramentas de enumeração pode ser considerada uma invasão e é ilegal em muitos países e jurisdições.</p>
            <p><strong>Dependências:</strong> O <code>enum4linux</code> geralmente requer Perl e pode precisar de outros módulos Perl. Verifique a documentação no repositório clonado para qualquer dependência adicional que possa ser necessária.</p>
        </section>
    </div>
</body>
</html>


nmap -sV -sC -Pn 10.10.80.211

smbclient //ipadress/folder -U user -p 445

nc -lvp

