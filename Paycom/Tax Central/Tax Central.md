We have a DataTable called Tax Codes that represents the database table and controls how it is displayed across the front-end.

A table will hold an array of Records for current and pending data, which will be displayed in the PowerTable. (Or, depending on how DataContext is built, it might just store a reference to objects in the data reducer). Look into something like a TableFactory with a static renderTable() function. If data is stored in a reducer, we don’t need to keep a table loaded in memory.

We have a Record called Tax Code that represents a row in the db table. Record handles functionality like equals() and toString() and toRow(). It also stores data of a type:

We have a type, Tax Code that represents a piece of data stored in a row. The type will declare the exact shape of the data and nothing else.

So the Table, Tax Code, will determine how the table is displayed in TUC and how the create form is displayed in TCC side drawer.

A user accesses TUC and selects Tax Codes. Table.get(‘TaxCode’) will construct a new Tax Codes object, which will send CurrentDataTable its columnMap while checking DataContext to see if it has any tax codes data. If not, it will call the API with table.getData() and store that in data context and send it to currentDataTable. In this process, each Tax Code Record will call .row() to build the row data array that power table needs. Dependencies will also be called and stored in data context.

When the user clicks on “Create Tax Code” and opens the side drawer, the Tax Code DataTable class will send its columnMap to render the Create form and load any required dependencies and validations (front-end and API side)