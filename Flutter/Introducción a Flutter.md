# Introducción a Flutter

## 1. Flutter y Dart

*Flutter* es un *SDK* (Software Development Kit), una colección de herramientas de desarrollo, creada por Google.
Su principal característica es que permite desarrollar aplicaciones nativas tanto para Android como IOS a través de un mismo *codebase* (base de código) utilizando solo un lenguaje de programación, *Dart*.

*Flutter* utiliza como unidad funcional componentes llamados *Widgets*, que no son más que bloques de UI (User Interface) reutilizables y personalizables.

Por otro lado, *Dart* es un lenguaje de programación también creado por Google que se centra en la creación de interfaces de usuario front-end.

## 2. Cómo funciona

Con *Flutter*, todo es un *widget*. Cada uno de los componentes de la aplicación móvil son *widgets*. Los más grandes involucran pequeños widgets y otros pequeños son más bien independientes. Al final de cuentas, la aplicación en si misma es un gran *widget tree*. 

Con *Flutter* solo es necesario desarrollar la aplicación una única vez, utilizando *Dart* y los *widgets* propios de *Flutter*.
Al momento de compilar la aplicación, lo que hace el *SDK* de *Flutter* es convertir el código escrito en *Dart* en código nativo tanto para Android como para IOS. Por lo tanto, el *codebase* final no es lo que fue desarrollado en Dart, sino más bien la traducción de ese código en los distintos lenguajes nativos.

*Flutter* permite hacer diferencia entre las versiones de Android e IOS, en caso de ser necesario o requerido, *Flutter* permite desarrollar dos productos finales distintos, o al menos no exactamente idénticos. 

El principal beneficio que se obtiene de esto, es que es posible crear código altamente optimizado y de alto rendimiento para ambos ambientes utilizando solo un lenguaje de programación, sin embargo, la traducción realizada por el *SDK* no se limita a los componentes nativos de ambas plataformas. *Flutter* posee una implementación personalizada, lo que significa que puede controlar cada pixel en pantalla, otorgándolo mucho control sobre los elementos y un alto grado de flexibilidad.

## 3. Elementos