# DocReactNative
O projeto DocReactNative trata-se de uma documentação geral sobre os apps: omnistack-mobile, SENAI-IBGE, YouFlix, CoronaAppBack e CoronaApp.

**Autor**

Foto | Nome | GitHub | Likedin | E-mail
---- | ---- | ------ | ------- | ------
<img src="https://avatars1.githubusercontent.com/u/56510921?s=400&u=7896f90f57edb9075a897ef19e6fb41e047d62c5&v=4" width="100px"> | Emanuel Oliveira Salvador Souza | [Emanuel](https://github.com/EmanuelOSSouza) | [Linkedin](https://www.linkedin.com/in/emanuel-oliveira-souza-ba-ti058a125/) | contato.souza.emanuel@gmail.com

**Objetivo**

Desenvolver uma documentação que explique os componentes e estruturas utilizadas para a confecção dos projetos citados acima.

**Justificativa**

Essa documentação faz parte de uma atividade das aulas de Desenvolvimento Mobile do curso de Desenvolvimento de Sistemas do Senai.

# Segue abaixo os pré-requisitos, tecnologias, frameworks, APIs e comandos utilizado nos projetos.

**Pré-requisitos**

- Node JS
- Visual Studio Code

**Tecnologias**

- React Native
- NPM
- CSS

Frameworks:

- Expo CLI
- Axios

APIs:

- [Covid-19](https://covid19-brazil-api-docs.now.sh/)
- [IBGE](https://servicodados.ibge.gov.br/api/docs)
- [YouTube](https://developers.google.com/youtube)


**Comandos**

* Instalar o Expo-cli:

`npm install -g expo-cli`

* Inicializar uma aplicação

`expo init name_project`

* Instalar dependências

`npm install`

* Start na aplicação


### [omnistack-mobile](https://github.com/EmanuelOSSouza/omnistack-mobile)
  No projeto omnistack foi utilizado os seguintes componentes:
  
  - **React**
  > Conceito: Componente principal responsavel por carregar os outros componentes do react
  
  > Exemplo de uso: import React from 'react';
  
  > Video referencia:
  
  - View: 
  > Conceito: Trata-se de um contêiner que suporta onde pode ser utilizado para interagir com outros componetes. Comporta-se de forma semelhante a <div> no HTML.
  
  > Exemplo de uso: 
     " <View style={styles.container}><\View>"
  
  > Video referencia:
  
  
  - **Text: **
  > Conceito: Basicamente exibe textos. Comporta-se de forma semelhante a <p> no HTML.
  
  > Exemplo de uso:
   <Text style={[styles.incidentProperty, {marginTop:0}]}>ONG:</Text>
  
  > Video referencia:
  
  - **Image:**
  > Conceito: Exibe imagens que podem está localizadas localmente ou remotamante.
  
  > Exemplo de uso:
    <Image source={logoImg} />
    
  > Video referencia:
  
  
  - **TouchableOpacity **
  > Conceito:
  
  > Exemplo de uso:
    <TouchableOpacity style={styles.action} onPress = {sendMail}>
  
  > Video referencia:
  
  
  - **StyleSheet**
  > Conceito:
  
  > Exemplo de uso:  <Text style={styles.incidentValue}><\Text>
  
  > Video referencia:
  
  
  - **FlatList**
  > Conceito:
  
  > Exemplo de uso:
    <FlatList style={Styles.list} data={statesInfo} keyExtractor={state => state.id} renderItem={({ item }) => {
                return (
                    <TouchableOpacity onPress={() => { navigation.navigate('State', item); }} style={Styles.categoryButton}>
                        <Text style={Styles.titleButtonCategory}>{ item.state }</Text>
                    </TouchableOpacity>
                );
            }} />
  
  > Video referencia:
  
  
  - **useNavigation**
  > Conceito:
  
  > Exemplo de uso:
    function navigationBack(){
        navigation.goBack();
    }
    
  > Video referencia:
  
  
  - **axios**
  > Conceito:
  
  > Exemplo de uso:
    const Api = Axios.create({
    baseURL: 'http://192.168.1.104:3333'
    });
  
  > Video referencia:
  
  
  - **NavigationContainer**
  > Conceito:
  
  > Exemplo de uso:
      <NavigationContainer>
      </NavigationContainer>
  
  > Video referencia:
  
  
  - **createStackNavigator**
  > Conceito:
  
  > Exemplo de uso:
    const AppStack = createStackNavigator();
      ....
      <AppStack.Navigator headerMode='none' initialRouteName='Home'>
          <AppStack.Screen name='Home' component={Home} />
      </AppStack.Navigator>
      
  
  > Video referencia:
  
  
  - **Linking**
  > Conceito:
  
  > Exemplo de uso:
  Linking.openURL(`whatsapp://send?phone=${incident.whatsapp}&text=${message}`);
  
  > Video referencia:
  
  
  - **Feather**
  > Conceito:
  
  > Exemplo de uso:
      <Feather name="arrow-left" size={28} color="#E82041" />
  > Video referencia:
  
  
  
### [SENAI-IBGE](https://github.com/EmanuelOSSouza/SENAI-IBGE)

### [YouFlix](https://github.com/EmanuelOSSouza/YouFlix)

### [CoronaApp](https://github.com/EmanuelOSSouza/CoronaApp)

### [CoronaAppBack](https://github.com/EmanuelOSSouza/CoronaAppBack)


**[Referências](https://reactnative.dev/)**
