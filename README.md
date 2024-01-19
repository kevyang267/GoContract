# GoContract

This application provides a platform for clients and contractors to interact through the internet. It gives users the abilities to search for contractors, book services from contractors and give them ratings; it allows contractors to approve/decline bookings, view their ratings, view their current active bookings, and provide invoices to users through an email address.

## Overview of Architecture

The application involves four distinct entities: a service consumer, service registry, service provider, and a database instance.

### Service Registry:

The service registry is a central database that stores a list of services that are provided by the service provider. Services can be added or removed, which will be updated on the service registry.

### Service Consumer:

Contains two different GUIs: a Find Contractor Search Engine GUI and a Find Search Booked Clients GUI. The Find Contractor is a GUI that allows users to search through a list of contractors in the service registry. The Find Search Booked is a GUI that allows the user to search through the list of clients attached to them in the service registry.

### Service Provider

Contains 5 distrinct services: Add/Remove TradeService, Manage Booking Service, Contract Invoice Service, Book Contractor Service, and Rate Service. The service provider explicitly provides these services.

### Database

An IBM Db2 instance that allows the secure storage of hashed user credentials. This nosql database is also used to store information about bookings and invoice data.
