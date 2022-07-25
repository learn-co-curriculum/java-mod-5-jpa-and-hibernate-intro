# What is JPA and Hibernate?

## Learning Goals

- Explain what JPA is and why we use it.
- Explain Hibernate and how it relates to JPA.

## Introduction

The Jakarta Persistence API (JPA) is a standard specification that defines how
an ORM should interact with a relational database. It was introduced so that a
common interface could be used across different ORM solutions.

## The JPA Standard

The JPA standard has three main parts:

- **The API**: This defines interfaces that specify methods for interacting with
  the ORM provider. It’s located in the `jakarta.persistence` package.
- **JPQL:** The Java Persistence Query Language (JPQL) is a query language that
  can be used to make requests to objects.
- **Metadata:** Annotations over objects that are used to define mapping between
  objects and a relational database. For example, the `@Entity` annotation over
  a plain Java class is used to indicate that the class represents a single
  table in a relational database. The fields in this class represents the
  columns in the table.

## What is Hibernate?

The JPA defines a specification for interacting with a database but it doesn’t
provide any concrete implementations for managing objects. The JPA interfaces
are implemented by different providers who define how exactly the objects are
managed.

Hibernate is one of the most popular implementations of JPA. It is highly
performant, reliable, extensible, and a complete implementation of JPA. And it
has a large community because of its popularity which makes it easier to find
possible solutions.

## Conclusion

We learned about JPA which is a set of interfaces which standardizes object
relational mapping and that Hibernate is one of the most popular implementations
of the JPA standard. In the next few lessons, we will learn how to set up
Hibernate and create objects to communicate with a database.
