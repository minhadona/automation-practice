<h4 style="text-align: center;"><span style="color: #008080; font-size: 80px;"><strong>Instru&ccedil;&otilde;es:</strong></span></h4>
<h4 style="text-align: center;"><span style="color: #808080;"><strong>-------------------------------------------------------------------------------------</strong></span></h4>
<p>&bull; Tenha instalado em sua m&aacute;quina <strong>Python</strong> (vers&atilde;o mais atualizada dispon&iacute;vel),<strong> <a href="https://jupyter.org/install.html">jupyter notebook</a></strong> e <strong>Google Chrome</strong><br /><br />&bull; Clone este reposit&oacute;rio<br /><br />&bull; Verifique sua vers&atilde;o do chrome instalada ao clicar na sequ&ecirc;ncia ilustrada ao seguir:</p>
<h3><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/y0F8Kem.png" alt="" /></h3>
<p>&bull; Baixe o ChromeDriver na vers&atilde;o correspondente ao seu navegador atrav&eacute;s do link <a href="https://chromedriver.chromium.org/downloads">https://chromedriver.chromium.org/downloads</a><br /><br />&bull; Coloque o arquivo do ChromeDriver baixado agora no lugar do que est&aacute; localizado na pasta do reposit&oacute;rio (o script e o chromedriver.exe atualizado devem estar sempre na mesma pasta, como na imagem):</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/iutUAXH.png" alt="" /></p>
<p>&bull; Clique no caminho do reposit&oacute;rio, onde est&aacute; indicado com um ponto vermelho, &agrave; frente da seta:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/y8Eqq5h.png" /></p>
<p>&bull; Digite cmd, e d&ecirc; enter</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/BCFFSic.png" /></p>
<p>&bull; O terminal abrir&aacute;, digite <span style="color: #008080;">jupyter notebook</span> e d&ecirc; enter:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/w8P7qO5.png" /></p>
<p>&bull; Isto abrir&aacute; o jupyter notebook no seu navegador default. Selecione o arquivo automationpractice.ipynb</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/5gMycWy.png" /></p>
<p>&bull; Para rodar o script, execute todas as c&eacute;lulas superiores at&eacute; chegar na c&eacute;lula das importa&ccedil;&otilde;es e a chamada da fun&ccedil;&atilde;o principal, execute ela, e o script deve come&ccedil;ar a rodar abrindo o chrome, enquanto os logs aparecem no output do jupyter notebook:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/igGg9IF.png" /></p>
<p>&bull; Para executar os testes unit&aacute;rios, execute todas as celulas anteriores, <strong>EXCETO a de Execu&ccedil;&atilde;o do script</strong>, como chamada, execute a c&eacute;lula abaixo de 'Testes Unit&aacute;rios', como indicado a seguir:</p>
<p><img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.imgur.com/1ssCoTu.png" /></p>
<p>&nbsp;</p>
<p>&bull; Caso deseje inserir dados para que o script crie uma nova conta no site, coloque as informa&ccedil;&otilde;es desejadas no dicion&aacute;rio que est&aacute; no in&iacute;cio do main():</p>
<p><img src="https://i.imgur.com/6qyelFE.png" /></p>
<p>&nbsp;</p>
<h2><span style="color: #008080;"><strong>LEMBRE-SE QUE:&nbsp;&nbsp;</strong></span></h2>
<h2>ao trocar o dicion&aacute;rio do main() na primeira vez, o script criar&aacute; uma conta pra voc&ecirc; com aquelas informa&ccedil;&otilde;es, mas se voc&ecirc; rod&aacute;-lo novamente, quando ele tentar logar, verificar&aacute; que houve sucesso no login e indicar&aacute; que voc&ecirc; pode prosseguir &agrave;s compras sem necessidade de CRIAR nova conta, pois as credenciais utilizadas j&aacute; est&atilde;o cadastradas e a senha est&aacute; correta.</h2>
<p>&nbsp;</p>
<h4 style="text-align: center;"><span style="color: #008080; font-size: 80px;"><strong>Considera&ccedil;&otilde;es:</strong></span></h4>
<h4 style="text-align: center;"><span style="color: #808080;"><strong>-------------------------------------------------------------------------------------</strong></span></h4>
<p>&nbsp;</p>
<p><span style="color: #808080;">Devido &agrave; op&ccedil;&atilde;o de cria&ccedil;&atilde;o do script manualmente (sem frameworks), n&atilde;o deu tempo de fazer a parte da compra. Foquei ent&atilde;o, nos testes unit&aacute;rios dos cen&aacute;rios que s&atilde;o poss&iacute;veis simular com os retornos das fun&ccedil;&otilde;es contempladas no script. Escolhi este tipo de teste unit&aacute;rio pois ele permite que cen&aacute;rios bastante alterados seram criados para cada lap de teste, possibilitando passar diferentes tipos de par&acirc;metros para as chamadas das fun&ccedil;&otilde;es, o que facilita para prever o comportamento do script: </span></p>
<p><span style="color: #808080;">- se um<strong> usu&aacute;rio estivesse inputando as informa&ccedil;&otilde;es</strong> que s&atilde;o passadas para as fun&ccedil;&otilde;es e m&eacute;todos atrav&eacute;s de um arquivo ou formul&aacute;rio; </span></p>
<p><span style="color: #808080;">- se o site estiver fora do ar ou algum bot&atilde;o/mensagem de retorno tiver mudado de nome ou de identifica&ccedil;&atilde;o no elemento web, dentre outras situa&ccedil;&otilde;es que devem ter <strong>retornos informativos</strong> para facilitar o trabalho de quem estiver dando manuten&ccedil;&atilde;o/debuggando o c&oacute;digo;</span></p>
<p><span style="color: #808080;">- entre outras situa&ccedil;&otilde;es espec&iacute;ficas;</span></p>
<p><span style="color: #808080;"> Isto torna poss&iacute;vel <strong>manter a qualidade e a continuidade do suporte nas plataformas envolvidas</strong>. </span><span style="color: #808080;">Al&eacute;m do r&aacute;pido diagn&oacute;stico de eventuais problemas, com a flexibilidade de fazer pequenas altera&ccedil;&otilde;es para readaptar os testes antes de rodar cen&aacute;rios ap&oacute;s uma mudan&ccedil;a de c&oacute;digo.&nbsp;</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h4 style="text-align: center;"><span style="color: #008080; font-size: 80px;"><strong>Bugs:</strong></span></h4>
<h4 style="text-align: center;"><span style="color: #808080;"><strong>-------------------------------------------------------------------------------------</strong></span></h4>
<p>O &uacute;nico bug que foi poss&iacute;vel identificar neste per&iacute;odo de tempo foi o fato de que a tentativa de login com senha errada nem sempre &eacute; retornada com 'Invalid password' pelo site. &Agrave;s vezes o site retorna somente Authentication Failed. Como este cen&aacute;rio &eacute; atribu&iacute;do ao fato de que n&atilde;o h&aacute; conta criada com aquelas credenciais, o rob&ocirc; prossegue para cria&ccedil;&atilde;o de nova conta desnecessariamente, pois ao chegar na fun&ccedil;&atilde;o que efetiva o registro da conta, uma mensagem dizendo que este e-mail j&aacute; est&aacute; sendo usado por outra credencial aparece, portanto a cria&ccedil;&atilde;o de uma nova conta n&atilde;o d&aacute; certo, j&aacute; que um novo e-mail teria que ser usado para tal. </p>
<p>Seria necess&aacute;rio debuggar mais vezes para identificar se tem algum padr&atilde;o entre o cen&aacute;rio onde o site retorna uma mensagem realmente informativa com o erro de login (ex: invalid password) vs quando retorna uma mensagem generalizada de falha de autentica&ccedil;&atilde;o, que induz algoritmo ao erro, visto que outra decis&atilde;o est&aacute; setada para este caso.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

