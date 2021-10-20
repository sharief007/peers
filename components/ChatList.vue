<template>
    <!-- <v-card> -->
      <v-list subheader two-line class="overflow-y-auto" height="calc(100vh - 11rem)">
      <v-subheader>Recent Chats</v-subheader>
      <v-list-item v-for="(item,index) in items" :key="index" link>
        <v-list-item-avatar>
          <v-img src="https://images.unsplash.com/photo-1457449940276-e8deed18bfff?ixid=MnwxMjA3fDB8MHxzZWFyY2h8NHx8cHJvZmlsZXxlbnwwfHwwfHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=600&q=60"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title v-text="item.name"></v-list-item-title>
          <v-list-item-subtitle v-text="item.message"></v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action>
          <v-badge :content="item.new"></v-badge>
        </v-list-item-action>
      </v-list-item>
    </v-list>
    <!-- </v-card> -->
</template>

<script>
export default {
    name: 'ChatList',
    data() {
        return {
          items: [
              {
                "name": "Jenna Cochran",
                "message": "gravida. Aliquam tincidunt,",
                "new": 91
              },
              {
                "name": "Nita Giles",
                "message": "faucibus lectus, a sollicitudin orci",
                "new": 69
              },
              {
                "name": "Moana Simpson",
                "message": "pellentesque a, facilisis non, bibendum sed,",
                "new": 83
              },
              {
                "name": "Nita Watkins",
                "message": "scelerisque neque.",
                "new": 10
              },
              {
                "name": "Julie Hatfield",
                "message": "egestas. Aliquam nec enim. Nunc ut erat.",
                "new": 20
              },
              {
                "name": "Cleo Ford",
                "message": "Duis",
                "new": 98
              },
              {
                "name": "Yoshi Decker",
                "message": "tempus",
                "new": 14
              },
              {
                "name": "Caryn Moreno",
                "message": "a feugiat tellus lorem eu metus.",
                "new": 93
              },
              {
                "name": "Desirae Mann",
                "message": "justo eu arcu. Morbi",
                "new": 95
              },
              {
                "name": "Bree Chase",
                "message": "placerat.",
                "new": 98
              },
              {
                "name": "Barbara Bryant",
                "message": "ornare, facilisis eget, ipsum. Donec sollicitudin adipiscing ligula.",
                "new": 59
              },
              {
                "name": "Shelby Nguyen",
                "message": "ut mi. Duis risus odio, auctor vitae, aliquet nec, imperdiet",
                "new": 5
              },
              {
                "name": "Kaitlin Dale",
                "message": "justo. Proin non massa non ante bibendum ullamcorper. Duis cursus,",
                "new": 49
              },
              {
                "name": "Vanna Bentley",
                "message": "porttitor interdum. Sed auctor odio",
                "new": 33
              },
              {
                "name": "Jade Burke",
                "message": "arcu. Vestibulum ut eros non",
                "new": 62
              },
              {
                "name": "Allegra Fischer",
                "message": "eleifend nec, malesuada ut, sem. Nulla",
                "new": 41
              },
              {
                "name": "Adena Barnett",
                "message": "enim, sit amet ornare lectus justo eu arcu. Morbi sit",
                "new": 69
              },
              {
                "name": "Georgia Thomas",
                "message": "non ante bibendum",
                "new": 87
              },
              {
                "name": "Chloe Romero",
                "message": "ac metus vitae velit",
                "new": 76
              },
              {
                "name": "Colleen Bailey",
                "message": "fringilla mi lacinia mattis. Integer eu lacus. Quisque",
                "new": 21
              },
              {
                "name": "Evelyn Diaz",
                "message": "mattis velit justo nec ante. Maecenas mi felis, adipiscing fringilla,",
                "new": 83
              },
              {
                "name": "Clio Steele",
                "message": "sed",
                "new": 76
              },
              {
                "name": "Hyacinth Richardson",
                "message": "Nunc lectus",
                "new": 46
              },
              {
                "name": "Zephr Hendrix",
                "message": "aliquet magna a neque. Nullam ut",
                "new": 50
              },
              {
                "name": "Meredith Scott",
                "message": "mollis non, cursus",
                "new": 81
              },
              {
                "name": "Brianna Jacobson",
                "message": "tellus faucibus leo, in lobortis",
                "new": 36
              },
              {
                "name": "Kylie Atkinson",
                "message": "pretium et, rutrum non, hendrerit id, ante. Nunc mauris",
                "new": 57
              },
              {
                "name": "Teagan Robertson",
                "message": "eget odio.",
                "new": 7
              },
              {
                "name": "Irene Kim",
                "message": "vel turpis. Aliquam adipiscing lobortis risus. In",
                "new": 61
              },
              {
                "name": "Larissa Nelson",
                "message": "luctus aliquet",
                "new": 11
              },
              {
                "name": "Ella Wiggins",
                "message": "Mauris molestie pharetra nibh. Aliquam",
                "new": 22
              },
              {
                "name": "Xyla Merrill",
                "message": "purus,",
                "new": 52
              },
              {
                "name": "Myra Donovan",
                "message": "eu dolor egestas rhoncus. Proin nisl sem, consequat nec,",
                "new": 75
              },
              {
                "name": "Kylie Lott",
                "message": "pellentesque a, facilisis non, bibendum sed, est. Nunc laoreet lectus",
                "new": 58
              },
              {
                "name": "Ingrid Hayden",
                "message": "imperdiet dictum magna. Ut tincidunt",
                "new": 100
              },
              {
                "name": "Kaye Pace",
                "message": "Donec feugiat metus sit amet ante. Vivamus non lorem vitae",
                "new": 99
              },
              {
                "name": "Diana Dean",
                "message": "enim. Sed nulla",
                "new": 78
              },
              {
                "name": "Daryl Grimes",
                "message": "lacus. Quisque imperdiet, erat nonummy ultricies ornare,",
                "new": 66
              },
              {
                "name": "Carolyn Stephenson",
                "message": "tristique senectus et netus",
                "new": 59
              },
              {
                "name": "Eleanor Conner",
                "message": "sociis natoque penatibus et magnis dis parturient montes, nascetur",
                "new": 36
              },
              {
                "name": "Carla Hunt",
                "message": "sit amet ornare lectus justo eu arcu. Morbi sit amet",
                "new": 80
              },
              {
                "name": "Athena Mitchell",
                "message": "convallis ligula. Donec",
                "new": 53
              },
              {
                "name": "Iliana Skinner",
                "message": "ipsum primis in",
                "new": 40
              },
              {
                "name": "Paula Kemp",
                "message": "penatibus et magnis dis parturient montes, nascetur ridiculus mus. Proin",
                "new": 94
              },
              {
                "name": "Odessa Gaines",
                "message": "arcu. Vivamus sit",
                "new": 62
              }
            ]
        }
    }
}
</script>