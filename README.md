# README

## Crear un Proyecto en Ruby in Rails

```bash
rails new mi_proyecto
cd mi_proyecto
```

## Puedes Usar el Comando Server del CLI para lanzar un servidor web que se integra con tu aplicación local para realizar peticiones

```bash
rails server
```

## 1- Se Configura la Ruta mi_proyecto/config/routes.rb

```ruby
Rails.application.routes.draw do
  get 'home/index'
  
  root 'home#index' 
end
```

## 2- En la ruta mi_proyecto/app/controllers Se Crea un archivo llamado home_controller.rb y ingresando las clases con mayuscula UpperCamelCase
U

```ruby
# Definimos el controlador HomeController que hereda de ApplicationController
class HomeController < ApplicationController
  #Definims la Acción index que se ejecutará cuando se acceda a la ruta /home/index
  def index
   
  end
end
```

## 3 - En la ruta mi_proyecto/app/views/home/index.html.erb  = Se crea la carpeta home y los archivos de index

```html.erb
<h1> Bienvenido a la página de inicio </h1>
```

## ERB: Es el motor de templates que nos permite embeber código de ruby en cualquier documento de texto

## Una vista que será procesada por ERB es aquella cuya extension termina en .html.erb

## Principalmente podemos identificar 3 etiquetas reconocidas que nos permiten:

1- Colocar código de Ruby <% %>
2- Colocar código comentado de Ruby <% # %>
3- Colocar expresiones que seran reemplazadas por su resultado <%=%>
