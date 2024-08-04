<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Instalação do enum4linux no Debian </title>
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
        ul {
            list-style: none;
            padding: 0;
        }
        ul li {
            margin: 10px 0;
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
<pre><code>sudo apt install python python-pip</code></pre>
</li>
<li>
<strong>Baixar e Instalar o <code>enum4linux</code></strong>
<pre><code>sudo apt install git
git clone https://github.com/PowerShellMafia/PowerSploit.git
cd PowerSploit/Recon/enum4linux
chmod +x enum4linux.pl</code></pre>
</li>
<li>
<strong>Executar o <code>enum4linux</code></strong>
<pre><code>./enum4linux.pl <endereço_IP></code></pre>
Substitua <code><endereço_IP></code> pelo endereço IP do alvo que você deseja escanear.
</li>
</ol>
</section>
<section class="steps">
           <h2>Exemplo de Execução</h2>
           <pre><code>./enum4linux.pl 10.10.133.29</code></pre>
       </section>
       <section class="steps">
           <h2>Nota</h2>
           <p><strong>Permissões e Legislação:</strong> Sempre obtenha permissão antes de realizar qualquer varredura em redes ou sistemas. A execução não autorizada de ferramentas de enumeração pode ser considerada uma invasão e é ilegal em muitos países e jurisdições.</p>
       </section>
   </div>
 </body>
   </html>
```
