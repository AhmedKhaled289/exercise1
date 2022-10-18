# exercise1
E2E Application development

portal project that get data from url and pass it to 

ServiceLayer to be saved in database 

http://localhost:8081/swagger-ui.html   to show services and test it 

Hibernate create table  at oracle dataabse 

scripts

CREATE TABLE SYS.USERS
(
  ID          NUMBER(19)                        NOT NULL,
  EMAIL       VARCHAR2(255 CHAR),
  NAME        VARCHAR2(255 CHAR),
  PHONE       VARCHAR2(255 CHAR),
  USERNAME    VARCHAR2(255 CHAR),
  WEBSITE     VARCHAR2(255 CHAR),
  ADD_ID      NUMBER(19),
  COMPANY_ID  NUMBER(19),
  primary key (ID)

)

CREATE TABLE SYS.ADDRESS
(
  ADD_ID      INTEGER,
  STREET      VARCHAR2(255 BYTE),
  SUITE       VARCHAR2(255 BYTE),
  CITY        VARCHAR2(255 BYTE),
  ZIPCODE     VARCHAR2(255 BYTE),
  ADDRESS_ID  NUMBER(19),
   primary key (ADD_ID)
)

CREATE TABLE SYS.COMPANY
(
  COMPANY_ID    INTEGER,
  NAME          VARCHAR2(255 BYTE),
  BS            VARCHAR2(255 BYTE),
  CATCH_PHRASE  VARCHAR2(255 CHAR),
   primary key (COMPANY_ID)
)

CREATE TABLE SYS.GEO
(
  ADDRESS_ID  INTEGER,
  LAT         VARCHAR2(255 BYTE),
  LNG         VARCHAR2(255 BYTE),
  primary key (ADDRESS_ID)
)
