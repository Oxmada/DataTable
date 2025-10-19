# @oxmad/data-table-component

Composant React réutilisable pour afficher des tableaux de données avec **tri**, **recherche** et **pagination**.

## Installation

```bash
npm install @oxmad/data-table-component
# ou
yarn add @oxmad/data-table-component
```

## Exemple d'utilisation


```jsx

import React from "react";
import { DataTable } from "@oxmad/data-table-component";

const employees = [
  { id: 1, firstName: "John", lastName: "Doe", department: "HR" },
  { id: 2, firstName: "Jane", lastName: "Smith", department: "Finance" },
  { id: 3, firstName: "Alice", lastName: "Johnson", department: "IT" },
];

function EmployeesTable() {
  return (
    <DataTable
      data={employees}
      searchable
      sortable
      paginated
      rowsPerPageOptions={[5, 10, 20]}
      defaultRowsPerPage={5}
      className="my-table"
    />
  );
}

export default EmployeesTable;
```
## Options combinables

```jsx
<DataTable
  data={employees}
  searchable={true}
  sortable={true}
  paginated={true}
  rowsPerPageOptions={[5, 10, 15, 20]}
  defaultRowsPerPage={10}
  className="custom-table"
/>
```
