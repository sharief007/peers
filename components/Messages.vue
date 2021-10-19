<template>
    <div class="chat-box">
        <div v-for="(item) in messageItems" :class="item.sent? 'message-sent':'message-received'" :key="item.id">
            <div :class="item.sent? 'message-sent-content':'message-received-content'">{{item.message}}</div>
        </div>
    </div>
</template>

<script>
export default ({
    name: 'Messages',
    data() {
        return {
            messageItems: [
                {
                "id": "302C3273-541D-ADDD-7844-EFEDD8DE4EFB",
                "message": "molestie tortor nibh sit amet orci. Ut sagittis lobortis mauris. Suspendisse aliquet molestie tellus. Aenean egestas hendrerit neque.",
                "sent": true
                },
                {
                "id": "6F10B232-ADB3-F989-936C-5DC2D0576CC6",
                "message": "ut, sem. Nulla interdum. Curabitur dictum. Phasellus in felis. Nulla tempor augue ac ipsum. Phasellus vitae",
                "sent": false
                },
                {
                "id": "403EAE82-2736-003A-9C7C-C7355ED0D387",
                "message": "eu elit. Nulla facilisi. Sed neque. Sed eget lacus. Mauris non dui nec urna suscipit nonummy. Fusce fermentum fermentum arcu. Vestibulum ante",
                "sent": true
                },
                {
                "id": "EBB4BE7B-60EF-332C-A28B-28335F8F481C",
                "message": "facilisis non, bibendum sed,",
                "sent": false
                },
                {
                "id": "0348288F-2DD4-93CF-88F6-76BC9CA045E5",
                "message": "in faucibus orci luctus et ultrices posuere cubilia Curae; Phasellus ornare. Fusce mollis. Duis sit amet diam",
                "sent": true
                },
                {
                "id": "18926D66-D27A-BFB3-C5F5-A99171668F71",
                "message": "fames ac turpis egestas. Aliquam",
                "sent": false
                },
                {
                "id": "79ABA225-E7CB-B65A-E87C-B4D0A4587905",
                "message": "egestas nunc sed libero. Proin",
                "sent": true
                },
                {
                "id": "749D12EC-6DFB-B4CB-A53B-DB9F69F64411",
                "message": "fames ac turpis egestas. Aliquam fringilla cursus purus. Nullam",
                "sent": true
                },
                {
                "id": "28C0B7D1-9233-7DA9-E4D5-0835710CE6F3",
                "message": "at auctor ullamcorper, nisl arcu iaculis enim, sit amet ornare lectus justo eu arcu. Morbi sit amet massa. Quisque porttitor eros nec tellus. Nunc lectus",
                "sent": true
                },
                {
                "id": "ACA73286-AB44-9306-7FD8-747C04AE469B",
                "message": "dictum eleifend, nunc risus varius orci, in consequat enim diam vel arcu. Curabitur ut odio vel est tempor",
                "sent": false
                },
                {
                "id": "F16A19A0-23E8-8D2C-C7B3-67700F3E00B5",
                "message": "ultrices",
                "sent": true
                },
                {
                "id": "8E3F418E-F264-DE67-9F9D-980401FED879",
                "message": "lorem, auctor quis, tristique ac, eleifend vitae, erat. Vivamus nisi. Mauris nulla. Integer urna. Vivamus",
                "sent": false
                },
                {
                "id": "64A1B8D6-0593-BE6E-1D9F-8BD1EB5B6AAD",
                "message": "sem elit, pharetra ut, pharetra sed, hendrerit a, arcu. Sed et libero. Proin mi. Aliquam gravida mauris ut mi. Duis risus odio,",
                "sent": false
                },
                {
                "id": "F0172383-201E-4A34-EB79-1C2C8D42ACBA",
                "message": "vitae purus gravida sagittis. Duis gravida. Praesent eu nulla at sem molestie sodales.",
                "sent": false
                },
                {
                "id": "70E43831-709A-6A19-2923-9EFF6817C5AE",
                "message": "sagittis augue, eu tempor erat",
                "sent": true
                },
                {
                "id": "608CAD57-3857-4197-FF2B-84ABB6B144BE",
                "message": "lobortis tellus justo",
                "sent": false
                },
                {
                "id": "C7C924B9-DDDC-ACEC-C48D-030F92BD3965",
                "message": "pede. Nunc sed orci lobortis augue scelerisque",
                "sent": true
                },
                {
                "id": "58857F54-0BA6-61B7-CF1E-315751F044AE",
                "message": "id, libero. Donec consectetuer mauris id sapien. Cras dolor dolor, tempus non, lacinia at, iaculis quis, pede. Praesent eu",
                "sent": true
                },
                {
                "id": "73CC0033-74D9-B553-C5C1-98DAF007C62B",
                "message": "eget tincidunt dui augue",
                "sent": false
                },
                {
                "id": "5FBB9297-A394-CFD8-CD12-733C077C8573",
                "message": "bibendum ullamcorper. Duis cursus, diam at",
                "sent": true
                },
                {
                "id": "2BAEEDF5-372C-4208-CE11-FA3742CA2A87",
                "message": "erat",
                "sent": true
                },
                {
                "id": "09372D2D-316D-6315-CFEB-D704B5A444CB",
                "message": "Sed eu eros. Nam consequat dolor vitae dolor. Donec fringilla. Donec feugiat metus sit amet ante. Vivamus non",
                "sent": true
                },
                {
                "id": "D0CCBC57-1A44-F7C1-1412-BFE8DD7EFC9D",
                "message": "magnis",
                "sent": false
                },
                {
                "id": "EE6919DE-0BD8-3480-1C04-EDF57FE8D0F8",
                "message": "pharetra ut, pharetra sed, hendrerit a, arcu. Sed et libero. Proin mi. Aliquam gravida",
                "sent": true
                }
            ]
        }
    }
})
</script>

<style scoped>
.chat-box {
  flex: 1;
  overflow-y: auto;
  min-height: calc(100vh - 8rem);
  max-height: calc(100vh - 8rem);
  padding: 0 10px;
}
.message-sent {
  padding: 5px;
	display: grid;
	grid-template-columns: 85%;
	justify-items: end;
    border-radius: 15px 0 15px 15px;
    justify-content: end;
}
.message-received {
  padding: 5px;
	display: grid;
	grid-template-columns: 85%;
    justify-items: start;
    border-radius: 0px 15px 15px 15px;
}
.message-sent-content {
  border-radius: 15px 15px 0px 15px;
  background-color: #0275d8;
  color: white;
  padding: 5px 10px;
}
.message-received-content {
  border-radius: 0px 15px 15px 15px;
  background-color: grey;
  padding: 5px 10px;
}
</style>