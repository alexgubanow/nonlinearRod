# phd_articles
My work on nonlinear rod article
Draft content of article:
FEM explisit(abaqus) and MSM
Введение и постановка задачи
В расчете целого клапана берется один стержень, 
существующие варианты расчетов всей системы и как в них рассчитывается хорда
Как движется кровь, описать механику (давление и скорость) 
Cравнить преимущества от расчета давления от скорости
Цель- сравнить один стержень и систему стержней
Хорда описана ломаной линией из элементов первого порядка
расчет давления жидкости от скорости на всю длину элемента под углом от направления жидкости

Понятие линейной деформации, допущения, понятия и эфекты
Нелинейное деформ стержня, по времени
Описать допущение что модуль упрогости = нелинейность 

Движение в жидкости

Движение узлов 
Описать силы в узлах от стержней
Учет напрвления элементов

Методы интегрирования

Результаты, как двигается, численные показатели силы


To get working VScode+Latex+WSL


    "latex-workshop.latex.tools": [
        {
            "name": "latexmk",
            "command": "latexmk",
            "args": [
                "--shell-escape", // added arg to default
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "%DOC%"
            ]
        },
        {
            "name": "pdflatex",
            "command": "pdflatex",
            "args": [
                "--shell-escape", // added arg to default
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "%DOC%"
            ]
        },
        {
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
            ]
        }
    ],
	
	
	
wget http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
tar xvzf install-tl-unx.tar.gz
cd 
sudo ./install-tl
PATH=/usr/local/texlive/2019/bin/x86_64-linux:$PATH; export PATH
MANPATH=/usr/local/texlive/2019/texmf-dist/doc/man:$MANPATH; export MANPATH
INFOPATH=/usr/local/texlive/2019/texmf-dist/doc/info:$INFOPATH; export INFOPATH
sudo apt install texlive-bibtex-extra
sudo apt install texlive-latex-extra
sudo apt install texlive-science
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt-get update
sudo apt-get install inkscape
sudo apt install pdflatex
