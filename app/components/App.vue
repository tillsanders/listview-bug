<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!"/>
        <GridLayout columns="*" rows="*">
            <ListView for="doctor in doctors">
                <v-template>
                    <Label :text="`${doctor.incarnation}, ${doctor.actor}`" />
                </v-template>
            </ListView>
        </GridLayout>
    </Page>
</template>

<script >
  export default {
    data() {
      return {
        doctors: [
            { incarnation: '1', actor: 'William Hartnell' },
            { incarnation: '2', actor: 'Patrick Troughton' },
            { incarnation: '3', actor: 'Jon Pertwee' },
            { incarnation: '4', actor: 'Tom Baker' },
            { incarnation: '5', actor: 'Peter Davison' },
            { incarnation: '6', actor: 'Colin Baker' },
            { incarnation: '7', actor: 'Sylvester McCoy' },
            { incarnation: '8', actor: 'Paul McGann' },
            { incarnation: 'War', actor: 'John Hurt' },
            { incarnation: '9', actor: 'Christopher Eccleston' },
            { incarnation: '10', actor: 'David Tennant' },
            { incarnation: '11', actor: 'Matt Smith' },
            { incarnation: '12', actor: 'Peter Capaldi' },
            { incarnation: '13', actor: 'Jodie Whittaker' },
        ],
      }
    }
  }
</script>

<style scoped>
    ActionBar {
        background-color: #53ba82;
        color: #ffffff;
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }
</style>
