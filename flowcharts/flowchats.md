```plantuml

@startuml

!theme amiga
title USER LOGIN

start
:Login as user;
repeat :Enter username and password;
:Authentification;
if(Authentification succeeded?) then (Yes)
:User is logged in;
stop
else (No)
if (Account was found?) then (Yes)
:Display error message;
else (No)
:Display sign up message;
stop

@enduml

```

```plantuml

@startuml

!theme amiga
title LIBRARIAN LOGIN


start
:Login as librarian;
repeat :Enter username and password;
:Authentification;
if(Authentification succeeded?) then (Yes)
:Librarian is logged in;
stop
else (No)
if (Account was found?) then (Yes)
:Show error message;
else (No)
:Not a librarian message;
stop

@enduml

```

```plantuml

@startuml

!theme amiga
title SIGN UP

start
:Sign up;
:Enter username;
repeat :Enter email;
backward:Error message;
repeat while (Is email valid?) is (No)
->Yes;
repeat :Enter password;
backward:Error message;
repeat while (Is password valid?) is (No)
->Yes;
:Generate Id;
:Account created;
stop

@enduml

```

```plantuml

@startuml

!theme amiga
title BORROW BOOK

start

@enduml

```
