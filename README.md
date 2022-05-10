# Template LaTeX para Trabalho de Conclusão de Curso da Universidade Federal do Oeste do Pará (UFOPA)

Este template LaTeX é baseado no Guia para Elaboração e Apresentação da Produção Acadêmica da UFOPA.O objetivo é padronizar os trabalhos acadêmicos produzidos na instituição, evitar plágios por falta de referenciamento correto da bibliografia e orientar a aplicação das diretrizes da Associação Brasileira de Normas Técnicas (ABNT).

Acesse o guia pelo Link : http://www.ufopa.edu.br/media/file/site/sibi/documentos/2020/b63bb8ebd08275c45d83368a436acfa1_w8bDoq2.pdf

Customização da classe abnTeX2: https://github.com/abntex/abntex2

# Editar
No arquivo principal "main.tex" estão todas as inclusões das partes do trabalho.Utilize um editor de textos de sua preferência (recomendável ATOM ou GEDIT) para editar os arquivos .tex. Todas as seções do trabalho são auto-explicativas bastando seguir as orientações de cada arquivo.

As referências devem ser inseridas no arquivo "bibliografia.bib" e serão incluídas na seção de referências do trabalho caso sejam citadas no corpo do trabalho. Podem ser inseridas todas as referências desejadas no arquivo "bibliografia.bib" com intuito de formar uma base de dados, estas referências não aparecerão no trabalho a menos que sejam citadas.Caso deseje pode ser utilizado algum software de gestão de referências para gerar automaticamente o arquivo "bibliografia.bib" (recomendável JabRef).

# Dicas
Veja a seguir como inserir alguns elementos no seu texto.

### Como inserir uma Tabela
```tex
\begin{table}[h!]
	\centering
	\Caption{\label{tab:label_da_tabela} Legenda da Tabela}
	\UFCtab{}{
		\begin{tabular}{ccll}
			\toprule
	    		Quisque & pharetra & tempus & vulputate \\
			\midrule \midrule
				E1 & Complete coverage & Both splice sites \\
				E2 & Complete coverage & Both splice sites \\
				E3 & Partial coverage & Both splice sites & Both \\
				E4 & Partial coverage & One splice site & Both \\
				E5 & Complete or coverage & No splice & Both \\
				E6 & No coverage & No splice sites\\
			\bottomrule
		\end{tabular}
	}{
		\Fonte{Elaborado pelo autor}
    }
\end{table}
```

### Como inserir um Quadro
```tex
\begin{quadro}[h!]
	\centering
	\Caption{\label{qua:label_do_quadro} Legenda do Quadro}
	\UFCqua{}{
		\begin{tabular}{|c|c|}
			\hline
			Quisque & pharetra \\
			\hline
			E1 & Complete coverage  \\
			\hline
			E2 & Complete coverage \\
			\hline
		\end{tabular}
	}{
		\Fonte{Elaborado pelo autor}
	}
\end{quadro}
```

### Como inserir uma figura
```tex
\begin{figure}[h!]
	\centering
	\Caption{\label{fig:label_da_figura} Legenda da Figura}
	\UFCfig{}{
	    \includegraphics[width=8cm]{figuras/figura-1}
	}{
	    \Fonte{Elaborado pelo autor}
	}
\end{figure}
```

### Como inserir uma alínea
```tex
\begin{alineas}
	\item Lorem ipsum dolor sit amet;
    \item Praesent vitae nulla varius;
	\item Praesent quis erat eleifend;
	\item Mauris facilisis odio eu:
	\begin{subalineas}
		\item Integer non lacinia magna;
		\item Proin mattis placerat risus.
	\end{subalineas}
\end{alineas}
```

### Como criar Capítulos
```tex
\chapter{Fundamentação Teórica}
\label{cap:fundamentacao-teorica}
```

### Como criar Seções
```tex
% Seções Secundárias
\section{Objetivo Geral 2}
\label{sec:objetivo-geral-2}

% Seções Terciárias
\subsection{Objetivo Geral 3}
\label{sec:objetivo-geral-3}

% Seções Quaternárias
\subsubsection{Objetivo Geral 4}
\label{sec:objetivo-geral-4}

% Seções Quinárias
\subsubsubsection{Objetivo Geral 5}
\label{sec:objetivo-geral-5}
```

### Como inserir um algoritmo
```tex
\begin{algorithm}[h!]
	\SetSpacedAlgorithm
	\caption{\label{alg:algoritmo_de_colonica_de_formigas}Algoritmo de Otimização por Colônia de Formiga}
	\Entrada{Entrada do Algoritmo}
	\Saida{Saida do Algoritmo}
	\Inicio{
		Atribua os valores dos parâmetros\;
		Inicialize as trilhas de feromônios\;
		\Enqto{não atingir o critério de parada}{
			\Para{cada formiga}{
				Construa as Soluções\;
			}
			Aplique Busca Local (Opcional)\;
			Atualize o Feromônio\;
		}
	}
\end{algorithm}
```

### Aviso: Este modelo não é oficial, apenas compartilho o modelo que chegou em minhas mãos após modificá-lo para maior praticidade de uso pessoal.
