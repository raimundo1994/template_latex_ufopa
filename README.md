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
\caption{\label{tab:Elemento} Tabela com valores  energéticas e fotopicos.}

	\begin{tabular}{ccll}
		\toprule
		Elemento & Intervalo Energético (MeV) & Fotopico (MeV) & Isótopo \\
		\midrule \midrule
		Pótassio &1.37-1.57 & 1.46 & $K^{40}$ \\
		Urânio & 1.66-1.86 & 1.76  & $Bi^{214}$  \\
		Tório & 2.41-2.81 & 2.61 &$Tl^{208}$ \\
		Contagem Total & 0.42-2.81 & - & - \\
		\bottomrule
	\end{tabular}
	
\legend{Fonte: Modificada de \citeonline{iaea2003guidelines,ferreira2016gamaespectrometria}.}

\end{table}
```

### Como inserir um Quadro
```tex
\begin{quadro}[ht]
	
	\caption{\label{aerogeofísico} Levantamento aerogeofísico Tucuruí (1097).}
	
	\begin{tabular}{ |l|l|l| }
		\hline
		\multicolumn{3}{ |c| }{PROJETO AEROGEOFISICO TUCURUÍ- (PROJETO 1097)} \\
		\hline
		\multirow{7}{*}{AQUISIÇÃO DE DADOS}
		&Ano de aquisição & 2010 \\
		&Velocidade de voo&266 Km/h \\
		&Altura de voo&100 m	 \\
		&Espaçamento entre linhas de voo&500 m\\
		&Orientação das linhas de voo & N-S\\
		&Espaçamento entre linhas de controle&10 Km\\
		&Orientação das linhas de controle&E-W\\
		\hline
		\multirow{4}{*}{MÉTODO GEOFÍSICO}
		& Magnetometria-Taxa de amostragem& 0,1 s \\
		& Aeromagnetomêtro & Scintrex CS-3/0,001nT\\
		& Gamaespectrometria-Taxa de amostragem& 1,0 s\\
		& Aerogamaespectrômetro&Exploranium GR-820 \\
		\hline
	\end{tabular}
	\vspace{1mm}
	
	\legend{Fonte: Do autor}
	
\end{quadro}
```

### Como inserir uma figura
```tex
\begin{figure}[!h]

	\caption{\label{radiação} Espectros de radiação gama..}
	\vspace{-6mm}
	
	\begin{center}
		\includegraphics[scale=0.9]{imagens/figura_10.jpg}  
	\end{center}
	
	\vspace{-4mm}
	\legend{Fonte: Modificado de \citeonline{foote1969improvement,ribeiro2014aerogamaespectrometria} }
	
\end{figure}
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

## Aviso: Este modelo não é oficial, apenas compartilho o modelo que chegou em minhas mãos após modificá-lo para maior praticidade de uso pessoal.
