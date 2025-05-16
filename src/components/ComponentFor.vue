<template>
  <table>
    <thead>
    <tr>
      <th>Id</th>
      <th>Name</th>
      <th>Address</th>
      <th>Email</th>
      <th>Phone</th>
    </tr>
    </thead>
    <tbody>
    <tr v-for="person in people" v-bind:key="person.id">
      <td>{{person.id}}</td>
      <td>{{person.name}}</td>
      <td>{{person.address.street}}</td>
      <td>{{person.email}}</td>
      <td v-if="person.phone">
        {{person.phone}}
      </td>
      <td v-else>
        -
      </td>
    </tr>
    </tbody>
  </table>
</template>

<script >
  export default {
    name: 'ComponentFor',
    data() {
      return {
        showHeader: true,
        showName: false,
        firstName: 'Gabriel',
        lastName: 'Zorzi',
        acessLevel: 'admin',
        people: [{
          id: 1,
          name: "Leanne Graham",
          username: "Bret",
          email: "Sincere@april.biz",
          address: {
            street: "Kulas Light",
            suite: "Apt. 556",
            city: "Gwenborough",
            zipcode: "92998-3874",
            geo: {
              lat: "-37.3159",
              lng: "81.1496"
            }
          },
          website: "hildegard.org",
          company: {
            name: "Romaguera-Crona",
            catchPhrase: "Multi-layered client-server neural-net",
            bs: "harness real-time e-markets"
          }
        },
          {
            id: 2,
            name: "Ervin Howell",
            username: "Antonette",
            email: "Shanna@melissa.tv",
            address: {
              street: "Victor Plains",
              suite: "Suite 879",
              city: "Wisokyburgh",
              zipcode: "90566-7771",
              geo: {
                lat: "-43.9509",
                lng: "-34.4618"
              }
            },
            phone: "010-692-6593 x09125",
            website: "anastasia.net",
            company: {
              name: "Deckow-Crist",
              catchPhrase: "Proactive didactic contingency",
              bs: "synergize scalable supply-chains"
            }
          }]
      }
    }
  }
</script>