# Fix a XML with a tag without closing tag that should not be a tag (fixing integration problems)

The RegEx above is a "fix" for XML's that have tags with no closing tags. 

It will prevent to break aplications that convert XML to Hash/JSON.

RegEx: <([\s\d\w=\/"\':]*)>[\s\d\n\w;,.-=\/]*(<[\d\w;,.-=\/ ]*>)[\s\d\w;,.-=\/]*<\/\1>

Example of XML:

<Correcao>Quando a exigibilidade do ISSQN for <Exportacao> informar o pais da prestacao do servico.</Correcao>

# Corrigir uma tag, sem tag de fechamento, que não deveria ser uma tag (consertando problemas de integração)

O RegEx abaixo é um "fix" para XMLs que possuem tags que não fecham.

Isso irá prevenir que quebre aplicações que convertem XML para Hash/JSON

RegEx: <([\s\d\w=\/"\':]*)>[\s\d\n\w;,.-=\/]*(<[\d\w;,.-=\/ ]*>)[\s\d\w;,.-=\/]*<\/\1>

Exemplo de XML:

<Correcao>Quando a exigibilidade do ISSQN for <Exportacao> informar o pais da prestacao do servico.</Correcao>
