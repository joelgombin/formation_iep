# Introduction à shiny
Joël Gombin  

# Quand utiliser shiny

- interface utilisateur : app ou document interactif
- besoin d'interaction (output réagit à un changement d'input)
- ce besoin d'interaction ne peut pas être traité *côté client*
- voir par exemple [htmlwidgets](www.htmlwidgets.org) pour cas où pas besoin de shiny, i.e. pas besoin d'une logique serveur complexe


```r
library(networkD3)
data(MisLinks, MisNodes)
forceNetwork(Links = MisLinks, Nodes = MisNodes, Source = "source",
             Target = "target", Value = "value", NodeID = "name",
             Group = "group", opacity = 0.4)
```

<!--html_preserve--><div id="htmlwidget-516" style="width:960px;height:672px;" class="forceNetwork html-widget"></div>
<script type="application/json" data-for="htmlwidget-516">{"x":{"links":{"source":[1,2,3,3,4,5,6,7,8,9,11,11,11,11,12,13,14,15,17,18,18,19,19,19,20,20,20,20,21,21,21,21,21,22,22,22,22,22,22,23,23,23,23,23,23,23,23,23,24,24,25,25,25,26,26,26,26,27,27,27,27,27,28,28,29,29,29,30,31,31,31,31,32,33,33,34,34,35,35,35,36,36,36,36,37,37,37,37,37,38,38,38,38,38,38,39,40,41,41,42,42,42,43,43,43,44,44,45,47,48,48,48,48,49,49,50,50,51,51,51,52,52,53,54,54,54,55,55,55,55,55,55,55,55,55,55,56,56,57,57,57,58,58,58,58,58,59,59,59,59,60,60,60,61,61,61,61,61,61,62,62,62,62,62,62,62,62,63,63,63,63,63,63,63,63,64,64,64,64,64,64,64,64,64,64,65,65,65,65,65,65,65,65,65,65,66,66,66,66,66,66,66,66,66,67,68,68,68,68,68,68,69,69,69,69,69,69,69,70,70,70,70,70,70,70,70,71,71,71,71,71,71,71,71,72,72,72,73,74,74,75,75,75,75,75,75,75,76,76,76,76,76,76,76],"target":[0,0,0,2,0,0,0,0,0,0,10,3,2,0,11,11,11,11,16,16,17,16,17,18,16,17,18,19,16,17,18,19,20,16,17,18,19,20,21,16,17,18,19,20,21,22,12,11,23,11,24,23,11,24,11,16,25,11,23,25,24,26,11,27,23,27,11,23,30,11,23,27,11,11,27,11,29,11,34,29,34,35,11,29,34,35,36,11,29,34,35,36,37,11,29,25,25,24,25,41,25,24,11,26,27,28,11,28,46,47,25,27,11,26,11,49,24,49,26,11,51,39,51,51,49,26,51,49,39,54,26,11,16,25,41,48,49,55,55,41,48,55,48,27,57,11,58,55,48,57,48,58,59,48,58,60,59,57,55,55,58,59,48,57,41,61,60,59,48,62,57,58,61,60,55,55,62,48,63,58,61,60,59,57,11,63,64,48,62,58,61,60,59,57,55,64,58,59,62,65,48,63,61,60,57,25,11,24,27,48,41,25,68,11,24,27,48,41,25,69,68,11,24,27,41,58,27,69,68,70,11,48,41,25,26,27,11,48,48,73,69,68,25,48,41,70,71,64,65,66,63,62,48,58],"value":[1,8,10,6,1,1,1,1,2,1,1,3,3,5,1,1,1,1,4,4,4,4,4,4,3,3,3,4,3,3,3,3,5,3,3,3,3,4,4,3,3,3,3,4,4,4,2,9,2,7,13,1,12,4,31,1,1,17,5,5,1,1,8,1,1,1,2,1,2,3,2,1,1,2,1,3,2,3,3,2,2,2,2,1,2,2,2,2,1,2,2,2,2,2,1,1,1,2,3,2,2,1,3,1,1,3,1,2,1,2,1,1,1,3,2,1,1,9,2,2,1,1,1,2,1,1,6,12,1,1,21,19,1,2,5,4,1,1,1,1,1,7,7,6,1,4,15,5,6,2,1,4,2,2,6,2,5,1,1,9,17,13,7,2,1,6,3,5,5,6,2,4,3,2,1,5,12,5,4,10,6,2,9,1,1,5,7,3,5,5,5,2,5,1,2,3,3,1,2,2,1,1,1,1,3,5,1,1,1,1,1,6,6,1,1,2,1,1,4,4,4,1,1,1,1,1,1,2,2,2,1,1,1,1,2,1,1,2,2,3,3,3,3,1,1,1,1,1,1,1,1,1,1,1],"colour":["#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666","#666"]},"nodes":{"name":["Myriel","Napoleon","Mlle.Baptistine","Mme.Magloire","CountessdeLo","Geborand","Champtercier","Cravatte","Count","OldMan","Labarre","Valjean","Marguerite","Mme.deR","Isabeau","Gervais","Tholomyes","Listolier","Fameuil","Blacheville","Favourite","Dahlia","Zephine","Fantine","Mme.Thenardier","Thenardier","Cosette","Javert","Fauchelevent","Bamatabois","Perpetue","Simplice","Scaufflaire","Woman1","Judge","Champmathieu","Brevet","Chenildieu","Cochepaille","Pontmercy","Boulatruelle","Eponine","Anzelma","Woman2","MotherInnocent","Gribier","Jondrette","Mme.Burgon","Gavroche","Gillenormand","Magnon","Mlle.Gillenormand","Mme.Pontmercy","Mlle.Vaubois","Lt.Gillenormand","Marius","BaronessT","Mabeuf","Enjolras","Combeferre","Prouvaire","Feuilly","Courfeyrac","Bahorel","Bossuet","Joly","Grantaire","MotherPlutarch","Gueulemer","Babet","Claquesous","Montparnasse","Toussaint","Child1","Child2","Brujon","Mme.Hucheloup"],"group":[1,1,1,1,1,1,1,1,1,1,2,2,3,2,2,2,3,3,3,3,3,3,3,3,4,4,5,4,0,2,3,2,2,2,2,2,2,2,2,4,6,4,4,5,0,0,7,7,8,5,5,5,5,5,5,8,5,8,8,8,8,8,8,8,8,8,8,9,4,4,4,4,5,10,10,4,8]},"options":{"NodeID":"name","Group":"group","colourScale":"d3.scale.category20()","fontSize":7,"fontFamily":"serif","clickTextSize":17.5,"linkDistance":50,"linkWidth":"function(d) { return Math.sqrt(d.value); }","charge":-120,"opacity":0.4,"zoom":false,"legend":false,"nodesize":false,"radiusCalculation":" Math.sqrt(d.nodesize)+6","bounded":false,"opacityNoHover":0,"clickAction":null}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

# c'est quoi shiny ?

Un framework créé par Rstudio, libre, gratuit, pensé pour le web d'aujourd'hui (HTML5, CSS, JS), mais qui ne nécessite pas de connaître ces notions : ça reste du R, on se concentre sur le R.

[Extrêmement bien documenté](http://shiny.rstudio.com/), avec une communauté d'usagers dynamique, un développement rapide (cf. [gadgets](http://shiny.rstudio.com/articles/gadgets.html) et [addins](https://rstudio.github.io/rstudioaddins/) par exemple)... ça vaut le coût d'investir !

Peut être utilisé en local pour soi-même, pour des collaborateurs/étudiants usagers de R/Rstudio, pour des collaborateurs non usagers de R, pour un grand public comme format de présentation/restitution en tant que tel ou dans une page HTML.

Deux exemples parmi [tant](http://www.showmeshiny.com/) [d'autres](https://www.rstudio.com/products/shiny/shiny-user-showcase/) : [http://shiny.cepii.fr/risk-shocks-and-divergence/](http://shiny.cepii.fr/risk-shocks-and-divergence/) et [https://gallery.shinyapps.io/sampling_and_stderr/](https://gallery.shinyapps.io/sampling_and_stderr/)

# Pour comprendre : un exemple récurrent

[http://www.joelgombin.fr/shiny/LireMinInterieur/](http://www.joelgombin.fr/shiny/LireMinInterieur/)

Source complète :  [sur github](https://github.com/joelgombin/LireMinInterieur)

Fichier de test : [sur dropbox](https://www.dropbox.com/s/8uh7ua3htkmv55u/Reg_15_circo_T1.csv?dl=0) (régionales 2015)

# Inputs, outputs, server

Avant même de commencer à écrire une applicaton shiny, se demander :

- quels sont [les inputs](http://shiny.rstudio.com/tutorial/lesson3/) ? (valeurs fournies par l'utilisateur, par quel biais ? Formulaire, widgets, fichier, source externe...)
- quels sont les outputs ? (valeurs générées par l'application, qui réagissent aux modifications de l'input ? texte, [graphiques](http://shiny.rstudio.com/articles/images.html), [cartes](https://rstudio.github.io/leaflet/shiny.html), [tableau](http://shiny.rstudio.com/articles/datatables.html)...)
- parfois un input peut *aussi* être un output, et vice versa ! (exemple : tableau)
- quelles fonctions prenant les inputs comme paramètres produisent les outputs ?

# Une application shiny, ce sont deux fonctions

## Une fonction ui.R

qui détaille l'interface utilisateur : inputs, outputs, mise en forme (par défaut en utilisant [bootstrap](http://shiny.rstudio.com/tutorial/lesson2/), mais on peut si on veut utiliser d'autres templates/frameworks). 



```r
library(shiny)

shinyUI(fluidPage(
  titlePanel("Transformer les fichiers électoraux du ministère de l'Intérieur"),
    sidebarLayout(
    sidebarPanel(
      fileInput("file", label = h3("Sélectionner un fichier csv"), accept=c('text/csv', 'text/comma-separated-values,text/plain')),
      checkboxInput("header", label="Y a-t-il des titres aux colonnes ?", value=TRUE),
      radioButtons("separator", label="Séparateur", c("Virgule" = ",", "Point virgule" = ";")),
      radioButtons("decimal", label="Séparateur décimal", c("Virgule" = ",", "Point" = ".")),
      actionButton("load", "Lire le jeu de données"),
      conditionalPanel(
        condition = "input.load > 0",
        htmlOutput("selectCol"),
        textInput("keepnames", label="noms à donner aux colonnes conservées (doit inclure 'Inscrits' et 'Exprimés'"),
        htmlOutput("selectCol2"),
        numericInput("colStep", label="Combien y a-t-il de colonnes entre les colonnes contenant les nuances politiques ?", value=7, min=1, step=1),
        numericInput("gap", label="Combien y a-t-il de colonnes entre les colonnes avec les étiquettes et celles avec le nombre de voix ?", value=3, min=1, step=1),
        HTML("<BR>"),
        actionButton("validate", "Transformer le fichier")
        ),
      helpText(HTML("<BR><BR><p>Cette application a été développée par <a href='http://www.joelgombin.fr'>Joël Gombin</a>.</p><p>Le code source est disponible sur <a href='http://www.github.com/joelgombin/LireMinInterieur'>mon compte Github</a>.</p>"))
      ),
    mainPanel(
      tabsetPanel(id="tab",
        tabPanel("Fichier avant transformation", dataTableOutput(outputId="tableau_before"), value="before"),
        tabPanel("Fichier après transformation", dataTableOutput(outputId="tableau_after"), downloadButton(outputId="downloadData", label="Télécharger"), value="after"))
      ))
))
```

## une fonction server.R

qui spécifie [comment les outputs sont liés aux inputs](http://shiny.rstudio.com/articles/build.html). C'est là que tout se passe en réalité.


```r
library(shiny)
library(LireMinInterieur)

shinyServer(function(input, output, session) {
  df <- reactive({
    input$load
    isolate({
      if (input$load==0) df <- NULL
      else {
        # petit hack pour gérer l'encodage. Faut-il intégrer d'autres encodages ?
        df <- tryCatch(read.csv((input$file)$datapath, header=input$header, sep=input$separator, dec=input$decimal, stringsAsFactor=FALSE, check.names = FALSE),
                      error = function(c) read.csv((input$file)$datapath, header=input$header, sep=input$separator, dec=input$decimal, stringsAsFactor=FALSE, check.names = FALSE, fileEncoding="ISO8859-1"))  
        names(df) <- iconv(names(df), from="", to="UTF-8")
      }
    })
    return(df)
  })
  
  output$tableau_before <- renderDataTable({
    df()
  }, options=list(pageLength=10))
  
  
  output$selectCol <- renderUI({
    selectizeInput("keep", label="Quelles colonnes faut-il conserver en l'état ?", choices=names(df()), multiple=TRUE)
  })

  observe({
    updateTextInput(session, "keepnames", label="noms à donner aux colonnes conservées (doit inclure 'Inscrits' et 'Exprimés'", value=input$keep)
  })  
  
  
  output$selectCol2 <- renderUI({
    selectizeInput("colInit", label="Quelle est la première colonne dans laquelle sont situées les nuances politiques ?", choices=names(df()), multiple=FALSE)
  })
  

  # transfomation du jeu de données quand il change
  
  df_trans <- reactive({
    # est dépendant de input$validate
    input$validate
    if (input$validate == 0) return(NULL)
    # on isole la suite
    
    isolate({
      index <- match(input$colInit, names(df()))
      col <- (dim(df())[2] - index) %/% input$colStep
      df_trans <- lire(df(), keep=input$keep, col=seq(from=index, by=input$colStep, length.out=col), keep.names=strsplit(input$keepnames, split=",")[[1]], gap=input$gap)
    })
    return(df_trans)
  })
  
  output$tableau_after <- renderDataTable({
    df_trans()
  }, options=list(pageLength=10))
  
  output$downloadData <- downloadHandler(
    filename = function() {
      paste("data-", Sys.Date(), ".csv", sep="")
    },
    content = function(con) {
      write.csv(df_trans(), con, row.names=FALSE)
    }
  )
  
})
```


# Écrivez votre première application shiny

- pour commencer, réfléchissez à une application (simple !) en identifiant bien inputs, outputs et logique serveur
- partez d'une [interface utilisateur simple](http://shiny.rstudio.com/tutorial/lesson2/), créez un squelette de fichier `ui.R`
- identifiez [comment coder les inputs](http://shiny.rstudio.com/tutorial/lesson3/)
- identifiez [comment codes les outputs](http://shiny.rstudio.com/tutorial/lesson4/)
- décrivez la [logique serveur](http://shiny.rstudio.com/tutorial/lesson4/)
- utilisez google et/ou demandez-moi pour résoudre les difficultés !
