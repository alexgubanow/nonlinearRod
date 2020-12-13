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
	
	
```bash	
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt-get update
sudo apt install inkscape
sudo apt install texlive
sudo apt install texlive-bibtex-extra
sudo apt install texlive-latex-extra
sudo apt install texlive-science
sudo apt install latexmk
sudo apt install texlive-extra-utils
sudo cpan Log::Log4perl
sudo cpan Log::Dispatch::File
sudo cpan YAML::Tiny
sudo cpan File::HomeDir
```

suggeted extensions: Rewrap
