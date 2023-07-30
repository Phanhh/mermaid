@startuml

!define EX_ITEM_APP exchange_used_item_app
!define MODEL model
!define VIEW view
!define CONTROLLER controller

package EX_ITEM_APP {
  package MODEL {
    [User]
    [Product]
    [Order]
  }

  package VIEW {
    [Home]
    [ProductList]
    [ProductDetail]
    [Cart]
    [Login]
  }

  package CONTROLLER {
    [HomeController]
    [ProductController]
    [CartController]
    [AuthController]
  }
}

EX_ITEM_APP.MODEL --> EX_ITEM_APP.CONTROLLER
EX_ITEM_APP.VIEW --> EX_ITEM_APP.CONTROLLER

@enduml
