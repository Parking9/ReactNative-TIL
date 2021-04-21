# React Native 


#### #expo 설치

```npm install -g expo-cli```

node.js 전역에 expo-cli 설치



`expo init [프로젝트 파일명]`

프로젝트 만들기



`cd [프로젝트 이름]`



`expo login`

expo 계정으로 로그인



`npm start`

expo dev tool  열기. 서버 구동



--> App.js가 모바일로 출력됨.



### local image

```react
import {Image} from "react-native";

<Image
    source={require("./assets/icon.png")}
    style={{ width: 240, height: 240, marginBottom: 15 }}
/>
```



### button (opacity)

```react
import { TouchableOpacity,StyleSheet} from "react-native";

const Button = ({ onPress }) => {
  return (
    <TouchableOpacity
      activeOpacity={0.8}
      style={styles.button}
      onPress={onPress}
    >
      <Text style={styles.text}>버튼</Text>
    </TouchableOpacity>
  );
};

const styles = StyleSheet.create({
  button: {
    width: 60,
    height: 60,
    backgroundColor: "#fe5746",
    justifyContent: "center",
    alignItems: "center",
  },
  text: {
    color: "#fff",
  },
});
```

