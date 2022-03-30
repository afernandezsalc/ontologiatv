# ontologiatv
ontología de serie de tv
<? xml version="1.0"?>
<rdf:RDF xmlns="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#"
     xml:base="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv"
     xmlns:owl="http://www.w3.org/2002/07/owl#"
     xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
     xmlns:xml="http://www.w3.org/XML/1998/namespace"
     xmlns:xsd="http://www.w3.org/2001/XMLSchema#"
     xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#"
     xmlns:swrl="http://www.w3.org/2003/11/swrl#"
     xmlns:swrla="http://swrl.stanford.edu/ontologies/3.3/swrla.owl#"
     xmlns:swrlb="http://www.w3.org/2003/11/swrlb#">
    <owl:Ontology rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv">
        <rdfs:comment xml:lang="es">Television Series OWL Ontology " La que se Avecina"

 Autor: Antonio Fernández Salcedo</rdfs:comentario>
        <rdfs:etiqueta xml:lang="es">Television_series</rdfs:etiqueta>
        <owl:versionInfo xml:lang="es">Version 1.0</owl:versionInfo>
    </búho:Ontología>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
 Propiedades de anotación
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://swrl.stanford.edu/ontologies/3.3/swrla.owl#isRuleEnabled -->

    <owl:AnnotationProperty rdf:about="http://swrl.stanford.edu/ontologies/3.3/swrla.owl#isRuleEnabled"/>
    


    <!-- http://www.w3.org/2000/01/rdf-schema#sameAs -->

    <owl:AnnotationProperty rdf:about="http://www.w3.org/2000/01/rdf-schema#sameAs">
        <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2000/01/rdf-schema#label"/>
    </búho:AnotaciónPropiedad>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
 Propiedades del objeto
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:dominio rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:rango>
            <búho:Restricción>
                <owl:onProperty rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasInterpretated"/>
                <búho:calificadoCardanidad rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">1</búho:calificadoCardanalidad>
                <owl:onClass rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
            </búho:Restricción>
        </rdfs:rango>
        <rdfs:comment xml:lang="es">La propiedad Interpretacción indica exactamente el personaje que interpreta el actor de la Clase Actors</rdfs:comment>
    </búho:ObjectProperty>
    


    http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasNameEpisodes <!-- -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasNameEpisodes">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#SymmetricProperty"/>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#TransitiveProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdfs:range rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdfs:comment xml:lang="es">La propiedad Nombre de capitulo indica la nombre del capitulo de la clase Episodes en cada una de las Temporadas (Seasons)</rdfs:comment>
    </owl:ObjectProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasYearSeasons -->

    <owl:ObjectProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasYearSeasons">
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AsymmetricProperty"/>
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:range>
            <owl:Restriction>
                <owl:onProperty rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#hasYearSeasons"/>
                <owl:qualifiedCardinality rdf:datatype="http://www.w3.org/2001/XMLSchema#nonNegativeInteger">2</owl:qualifiedCardinality>
                <owl:onClass rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
            </owl:Restriction>
        </rdfs:range>
        <rdfs:comment xml:lang="es">La propiedad Años de las Temporadas indica exactamente 2 años de cada Temporada (Seasons)</rdfs:comment>
    </owl:ObjectProperty>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Data properties
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberQuota -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberQuota">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Cuota indica el porcentaje de la Audiencia</rdfs:comment>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberSpecteators -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberSpecteators">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Espectadores indica el número de espectadores que tiene la audiencia.</rdfs:comment>
    </owl:DatatypeProperty>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberseasons -->

    <owl:DatatypeProperty rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#numberseasons">
        <rdfs:domain rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
        <rdfs:comment xml:lang="es">La propiedad Numero de Temporada indica el número de Temporada de la serie</rdfs:comment>
    </owl:DatatypeProperty>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Classes
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Actores que puede tener instancias como el nombre de los actores</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase de Tipo de Audiencia puede tener instancias como acumulada, bruta, duplicada</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Premios, que puede tener instancias como mejor serie, mejor guion, mejor actor, mejor actriz, mejor serie de comedia, premio Sangay, premio Zapping, premio Pasión de Críticos</rdfs:comment>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Category:Television_series"/>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Medios de difusion que puede tener instancias como Telecinco, Amazon Prime Video, Disney +, Netflix, Atresplayer, YouTube</rdfs:comment>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Category:Series"/>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <owl:disjointWith rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
        <rdfs:comment xml:lang="es">Clase Comedia que puede tener instancias como comedia de situación</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Pais de origen que puede tener instacia como Spain</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Creadores que puede tener instancias con el nombre de los creadores</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Directores que puede tener instancias con el nombre de los directores</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Episodios puede tener instancias como número de episodio 11</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Final, que identifica la fecha de final de emision de la Temporada, puede tener una instancia como 22 de julio de 2007</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Generos que puede tener instancias genericas de los diferentes generos y mas ordenadamente tiene las subclases de Comedy y Humor</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <rdfs:comment xml:lang="es">Clase Humor que puede tener instacias como humor negro</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Lenguaje original que tiene instancia como Spanish</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Person que tiene subclases (Actores, Creadores, Directores, Productores, Guionista)</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Estreno que puede tener una instancia con la fecha de estreno de la temporada como 22 de abril de 2007</rdfs:comment>
        <rdfs:label xml:lang="es">Premier</rdfs:label>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Productores que puede tener instancias con el nombre de los productores</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Couta puede tener instancia como 23.3 %</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdfs:comment xml:lang="es">Clase Guionistas que pueden tener instancias con el nombre de los guionistas</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Temporadas, puede tener instancias como Temporada 4 (2009-2010), Temporada 12(2020-2022)</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators">
        <rdfs:subClassOf rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdfs:comment xml:lang="es">Clase Espectadores puede tener una instacia como 3.185.000</rdfs:comment>
    </owl:Class>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title -->

    <owl:Class rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
        <rdfs:comment xml:lang="es">Clase Titulo que puede tener instancia como La que se Avecina</rdfs:comment>
        <rdfs:label xml:lang="es">Title</rdfs:label>
        <rdfs:sameAs rdf:resource="https://dbpedia.org/page/Television_show"/>
    </owl:Class>
    


    <!-- http://www.w3.org/2002/07/owl#SerieTV -->

    <owl:Class rdf:about="http://www.w3.org/2002/07/owl#SerieTV">
        <rdfs:subClassOf rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
        <rdfs:comment xml:lang="es">Clase Serie de Television</rdfs:comment>
    </owl:Class>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Individuals
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Alberto_Caballero -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Alberto_Caballero">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Producers"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Screenwriters"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Amazon_Prime_Video -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Amazon_Prime_Video">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Atresplayer -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Atresplayer">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedia_de_situacion -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedia_de_situacion">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor_negro -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor_negro">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Jordi_Sánchez -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Jordi_Sánchez">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#La_que_se_Avecina -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#La_que_se_Avecina">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Laura_Caballero -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Laura_Caballero">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Directors"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Netflix -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Netflix">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spain -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spain">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spanish -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spanish">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Telecinco -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Telecinco">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#11-07-15 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#11-07-15">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#12-09-16 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#12-09-16">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2014.Premio_MiM_Series.Mejor_serie_de_comedia -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2014.Premio_MiM_Series.Mejor_serie_de_comedia">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_guion. -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_guion.">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_serie -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#2016.Premios_Iris.Mejor_serie">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#23.2 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#23.2">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3.000.000 -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#3.000.000">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators"/>
    </owl:NamedIndividual>
    


    <!-- http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Disney_+ -->

    <owl:NamedIndividual rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Disney_+">
        <rdf:type rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
    </owl:NamedIndividual>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // General axioms
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Audience"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Episodes"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Final"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Premiere"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Quota"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Spectators"/>
        </owl:members>
    </rdf:Description>
    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Country_origin"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Original_language"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        </owl:members>
    </rdf:Description>
    <rdf:Description>
        <rdf:type rdf:resource="http://www.w3.org/2002/07/owl#AllDisjointClasses"/>
        <owl:members rdf:parseType="Collection">
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Awards"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Broadcast_medium"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Seasons"/>
            <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
        </owl:members>
    </rdf:Description>
    


    <!-- 
    ///////////////////////////////////////////////////////////////////////////////////////
    //
    // Rules
    //
    ///////////////////////////////////////////////////////////////////////////////////////
     -->

    <rdf:Description rdf:about="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p">
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Variable"/>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S1</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Actors"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S3</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Comedy"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                        <rdf:first>
                            <rdf:Description>
                                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                                <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Humor"/>
                                <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                            </rdf:Description>
                        </rdf:first>
                        <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
                    </rdf:Description>
                </rdf:rest>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Genders"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Description>
    <rdf:Description>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S2</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:body>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Creators"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:body>
        <swrl:head>
            <rdf:Description>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:first>
                    <rdf:Description>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicate rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Person"/>
                        <swrl:argument1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Description>
                </rdf:first>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Description>
        </swrl:head>
    </rdf:Descripción>
    <rdf:Descripción>
        <swrla:isRuleEnabled rdf:datatype="http://www.w3.org/2001/XMLSchema#boolean">true</swrla:isRuleEnabled>
        <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string"></rdfs:comment>
        <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">S4</rdfs:label>
        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#Imp"/>
        <swrl:cuerpo>
            <rdf:Descripción>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:primero>
                    <rdf:Descripción>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicar rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#Title"/>
                        <swrl:argumento1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Descripción>
                </rdf:primero>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Descripción>
        </swrl:cuerpo>
        <swrl:cabeza>
            <rdf:Descripción>
                <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#AtomList"/>
                <rdf:primero>
                    <rdf:Descripción>
                        <rdf:type rdf:resource="http://www.w3.org/2003/11/swrl#ClassAtom"/>
                        <swrl:classPredicar rdf:resource="http://www.w3.org/2002/07/owl#SerieTV"/>
                        <swrl:argumento1 rdf:resource="http://www.semanticweb.org/antonio/ontologies/2022/2/serietv#p"/>
                    </rdf:Descripción>
                </rdf:primero>
                <rdf:rest rdf:resource="http://www.w3.org/1999/02/22-rdf-syntax-ns#nil"/>
            </rdf:Descripción>
        </swrl:cabeza>
    </rdf:Descripción>
</rdf:RDF>



<!-- Generado por la API de OWL (versión 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi -->
