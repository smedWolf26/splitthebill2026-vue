<script setup>
    import Header from './components/Header.vue'
    import Card from './components/Card.vue'
</script>

<template>
    <Header/>
    <Card>

        <form id="personForm" class="rowForm">
            <input id="personInput" type="text" placeholder="Add persons name"/>
            <button>Add Person</button>
        </form>

        <form id="expenseForm" class="rowForm">
             <input id="descInput" type="text" placeholder="Expense Description" />
             <input id="amountInput" type="number" placeholder="amount" />
             <select id="paidBySelect"></select>
             <button>Add Expense</button>
        </form>
        <section>
            <h3>People</h3>
            <ul id="peopleList" class="list"></ul>
        </section>

        <section>
            <h3>Expenses</h3>
                  <ul id="expenseList" class="list"></ul>
         
              
        </section>
            <h3>Total</h3>
            <p>
                Total Spent: <strong id="totalSpent" >$0.00</strong><br/>
                Split Per Person <strong id="splitAmount" >$0.00</strong>
            </p>
        <section>

        </section>
        <section class="summary">
            <h3>Summary</h3>
                <ul id="summaryList" class="list"></ul>
        </section>
  </Card>
</template>

<style scoped>
.rowForm {
    display: flex;
    gap: 10px;
    margin-bottom: 12px;
}

input, select {
    flex: 1;
    padding: 10px;
    border-radius: 10px;
    border: 1px solid #c7d2fe;

}

button {
    padding: 10px 14;
    border-radius: 10px;
    border: none;
    background-color: #403c87;
    color: #fff;
    cursor: pointer;
}



</style>
