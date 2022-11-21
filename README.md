# What is JPA and Hibernate?

## Learning Goals

- Define the Jakarta Persistence API (JPA) specification.
- Introduce Hibernate as a JPA implementation.

## Introduction

The **Jakarta Persistence API (JPA)** is a standard specification that defines how
an ORM should interact with a database. It was introduced so that a
common interface could be used across different ORM solutions.

In JPA, we define persistence rules based on Java classes and objects.
This is different that JDBC, which requires us to manually
translate from Java classes to relational tables and back again.

## The JPA Standard

The JPA standard has three main parts:

- **The API**: The API specifies methods for interacting with
  the ORM provider. It’s located in the `jakarta.persistence` package.
- **JPQL:** The **Java Persistence Query Language (JPQL)** is a query language that
  can be used to make data requests with objects.
- **Metadata:** Annotations are used to define a mapping between
  objects and a data store. For example, the `@Entity` annotation
  is used to indicate that a Java class represents a single
  table in a relational database. The fields in the class represents the
  columns in the table.

## What is Hibernate?

The JPA defines a specification for interacting with a database but it doesn’t
provide any concrete implementations for managing objects. The JPA interfaces
are implemented by different providers who define how exactly the objects are
managed.

**Hibernate** is one of the most popular implementations of JPA. It is highly
performant, reliable, extensible, and a complete implementation of JPA. It
has a large community because of its popularity which makes it easier to find
possible solutions.

## Conclusion

JPA which is a specification that provides standards for mapping objects
to a database. Hibernate is one of the most popular implementations
of the JPA standard. In the next few lessons, we will learn how to set up
Hibernate and create objects to persist in a database.


## Resources

- [Java Persistence API](https://download.oracle.com/otn-pub/jcp/persistence-2_1-fr-eval-spec/JavaPersistence.pdf?AuthParam=1669035788_55339cf2dd0c10154e6e956b139d31ee)    
- [JPA Service Specification](https://docs.osgi.org/specification/osgi.cmpn/8.0.0/service.jpa.html)       
- [Introduction to Java Persistence API](https://docs.oracle.com/javaee/6/tutorial/doc/bnbpz.html)  
- [Hibernate](https://hibernate.org/)  