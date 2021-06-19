<template>
  <div class="q-pa-md">
    <q-table
      title="Top Products"
      :data="data"
      :columns="columns"
      row-key="name"
    >
      <template v-slot:body="props">
        <q-tr :props="props">
          <q-td key="name" :props="props">
            {{ props.row.name }}
          </q-td>
          <q-td key="in_stock" :props="props">
            <q-badge color="green">
              {{ props.row.in_stock }}
            </q-badge>
          </q-td>
          <q-td key="sales" :props="props">
            <q-badge color="purple">
              {{ props.row.sales }}
            </q-badge>
          </q-td>
          <q-td key="profit" :props="props">
            <q-badge color="orange">
              {{ props.row.profit }}
            </q-badge>
          </q-td>
          <q-td key="loss" :props="props">
            <q-badge color="primary">
              {{ props.row.loss }}
            </q-badge>
          </q-td>
          <q-td key="discount" :props="props">
            <q-badge color="teal">
              {{ props.row.discount }}
            </q-badge>
          </q-td>
        </q-tr>
      </template>
    </q-table>
  </div>
</template>
<script>
export default {
  name:'Table',
  data () {
    return {
      columns: [
        {
          name: 'name',
          required: true,
          label: 'Name of the Product',
          align: 'left',
          field: row => row.name,
          format: val => `${val}`,
          sortable: true
        },
        { name: 'in_stock', align: 'center', label: 'In Stock', field: 'in_stock', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10) },
        { name: 'sales', label: 'Sales (%)', field: 'sales', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10) },
        { name: 'profit', label: 'Profit (%)', field: 'profit', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10) },
        { name: 'loss', label: 'Loss (%)', field: 'loss', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10) },
        { name: 'discount', label: 'Discount (%)', field: 'discount', sortable: true, sort: (a, b) => parseInt(a, 10) - parseInt(b, 10) }
      ],

      data: [
        {
          name: 'Product 1',
          in_stock: 159,
          sales: 6.0,
          profit: 24,
          loss: 4.0,
          discount: 87
        },
        {
          name: 'Product 2',
          in_stock: 237,
          sales: 9.0,
          profit: 37,
          loss: 4.3,
          discount: 129
        },
        {
          name: 'Product 3',
          in_stock: 262,
          sales: 16.0,
          profit: 23,
          loss: 6.0,
          discount: 337
        },
        {
          name: 'Product 4',
          in_stock: 305,
          sales: 3.7,
          profit: 67,
          loss: 4.3,
          discount: 413
        },
        {
          name: 'Product 5',
          in_stock: 356,
          sales: 16.0,
          profit: 49,
          loss: 3.9,
          discount: 327
        },
        {
          name: 'Product 6',
          in_stock: 375,
          sales: 0.0,
          profit: 94,
          loss: 0.0,
          discount: 50
        },
        {
          name: 'Product 7',
          in_stock: 392,
          sales: 0.2,
          profit: 98,
          loss: 0,
          discount: 38
        },
        {
          name: 'Product 8',
          in_stock: 408,
          sales: 3.2,
          profit: 87,
          loss: 6.5,
          discount: 562
        },
        {
          name: 'Product 9',
          in_stock: 452,
          sales: 25.0,
          profit: 51,
          loss: 4.9,
          discount: 326
        },
        {
          name: 'Product 10',
          in_stock: 518,
          sales: 26.0,
          profit: 65,
          loss: 7,
          discount: 54
        }
      ]
    }
  }
}
</script>