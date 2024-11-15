Segue o exercício. Não consegui terminar, eu consegui criar a pasta no diretório, mas nao salva nada, nao entendo. Fiz um exec no container,
e cirei manualmente o arquivo.txt teste e ele criou na pasta, mas quando guardo os dados da aplicação, não salva.
Não vi necessidade criar pod e service para o SQLITE visto que é nativo do django. Achei que poderia ser por nao ter o migrate,
criei um initcontainer para rodar as migrates e mesmo assim sem sucesso. Modifiquei o caminho do DATABASE, em settings e mesmo assim..
sem sucesso.

Poderia ter feito dinamicamente, mas achei que seria matar uma formiga com uma bazuca, não achei necessidade, porém manualmente nao consegui kk.
Pensei em criar um confimaps para passaro caminho do volume para o SQLITEM, mas também nao deu certo kk.
O volume foi criado, montado, verifiquei no LENS. Terça trocamos ideia. Valeu!

A  imagem do log está anexada.
