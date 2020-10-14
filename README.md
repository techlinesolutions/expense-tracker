
<div class="jumbotron text-center">
    <p align="center"><span style="font-family: 'Liberation Sans', serif;"><span
            style="font-size: xx-large;"><strong><H1>How to Create An Expense Tracker App in React Native</H1></strong></span></span>
    </p>
    <p class="western">&nbsp;</p>
    <p class="western" align="center">Author: Michael Ekeghe</p>
    <p class="western" align="center">A React Native Tutorial Project.</p>
    <p class="western" align="center">For the Facebook Developer Challenge 2020</p>

</div>
<div class="container">
    <div class="row">
        <div class="col-sm-6">
          
                    
                        ##Introduction

            <p class="western">Are you <span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Looking for a way to create an expense and budget tool that runs on your mobile device? Stop searching and lets create one.</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>This Expense Tracker is a simple, intuitive, stable and feature-rich app that is just designed for you. Everything you need at your fingertips to manage the expenditures, checkbook and budgets.</span></span></span><br/>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Get ready to track Your expenses and stick to a budget with this easy and efficient finance planning tool that we are about to create</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Are you ready? Lets dive in</span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <ol>
                <ol start="2">
                    <li>
                        <h2 class="western">Prerequisites</h2>
                    </li>
                </ol>
            </ol>
            <ul>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>Knowledge of Basic ES6 JavaScript or typescript</span></span></span>
                    </p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>A Text Editor (Atom/VS Code, or anyone anyone actually)</span></span></span>
                    </p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>A tiny bit of React Know how</span></span></span>
                    </p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>Node (versions 12.8 and above)</span></span></span>
                    </p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>Expo App downloaded from AppStore or Google Play Store</span></span></span>
                    </p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>Internet</span></span></span></p>
                </li>
                <li>
                    <p class="western"><span style="color: #333333;"><span
                            style="font-family: Roboto, Arial, sans-serif;"><span>API server (I used an API hosted on heroku)</span></span></span>
                    </p>
                </li>
            </ul>
            <p class="western">&nbsp;</p>

            <ol>
                <ol start="3">
                    <li>
                        <h2 class="western">Preliminary Set-up</h2>
                    </li>
                </ol>
            </ol>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>1. Make sure you have </span></span></span><span
                    style="color: #333333;"><span style="font-family: Roboto, Arial, sans-serif;"><span><u><strong>Nodejs</strong></u></span></span></span><span
                    style="color: #333333;"><span style="font-family: Roboto, Arial, sans-serif;"><span> set up and working on your machine. If you already have node installed on your machine, just move on to the next item.</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>For detailed instructions on how to install nodejs on your device, visit the link below</span></span></span>
            </p>
            <p class="western"><span style="color: #000080;"><span lang="zxx"><u><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>https://nodejs.org/en/download/package-manager/</span></span></span></u></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <ol>
                <ol start="4">
                    <li>
                        <h2 class="western"><span style="color: #000080;"><span lang="zxx"><span
                                style="color: #1c1c1c;">Summary of Instalation and set up</span></span></span></h2>
                    </li>
                </ol>
            </ol>
            <p class="western"><span style="color: #1c1c1c;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Assuming that you have Node 12 LTS or greater installed, you can use npm to install the Expo CLI command-line utility:</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>1. npm install -g expo-cli</span></span></span>
            </p>
            <p class="western"><a name="__DdeLink__56_3871871116"></a> <span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>2. expo init ExpenseTracker</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>3. cd ExpenseTracker</span></span></span></p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>4. expo start </span></span></span></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <ol>
                <ol start="5">
                    <li>
                        <h2 class="western">The Main The Main</h2>
                    </li>
                </ol>
            </ol>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>1. For this project, we are using Expo. Its a command-line tool that simplifies your react-native development and testing </span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Run the below commands to begin</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><strong>npm install -g expo-cli</strong></span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>2. Next we actually initialize or simply create the react-native base project</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>We do this by running the following command in your terminal window</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><strong>expo init ExpenseTracker</strong></span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/1.png" width="665" height="348" name="Image1" align="left" border="0"/></p>

            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><strong>3. chose the tabs(Typescript) template</strong></span></span></span>
            </p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/0.png" width="665" height="348" name="Image1" align="left" border="0"/></p>

            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span><strong>Once done</strong></span></span></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>4. Once done navigate to the new created projects&rsquo; directory</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>cd </span></span></span><span
                    style="color: #333333;"><span style="font-family: Roboto, Arial, sans-serif;"><span><strong>ExpenseTracker</strong></span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><strong>5.Run expo start in your terminal</strong></span></span></span>
            </p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/2.png" width="529" height="487" name="Image3" align="left" border="0"/></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><strong>6. </strong></span></span></span><span
                    style="color: #333333;"><span style="font-family: Roboto, Arial, sans-serif;"><span>Open the ExpenseTracker folder in your text editor and you will see a similar folder structure</span></span></span>
            </p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/3.png" width="195" height="380" name="Image4" align="left" border="0"/></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>

            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>7. now let's test our template app with the Expo app on your mobile device.</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>For Android users, </span></span></span></p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Launch the expo app </span></span></span></p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Click the scan button </span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Scan the QR code</span></span></span></p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>For iPhone /Ipad users</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Launch your Camera app</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>View the QR code</span></span></span></p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>The App template is automatically launched</span></span></span>
            </p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/4.jpg" width="151" height="252" name="Image5" align="left" border="0"/></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>8. install the moment component</span></span></span>
            </p>
            <pre class="western"><span style="color: #000000;"><span style="font-family: monospace, monospace;"><span
                    style="font-size: medium;">npm&nbsp;install&nbsp;--save&nbsp;moment&nbsp;react-moment</span></span></span></pre>
            <p class="western"><br/></p>
            <p class="western"><a name="user-content-timezone-support"></a>9. Install the
                react-native-modal-datetime-picker component<br/> <span style="color: #000000;"><span
                        style="font-family: monospace, monospace;"><span style="font-size: medium;">npm&nbsp;i&nbsp;react-native-modal-datetime-picker&nbsp;@react-native-community/datetimepicker</span></span></span>
            </p>
            <p class="western"><br/> <br/></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>9.Update the Navigation Menus</span></span></span>
            </p>
            <p class="western">&nbsp;</p>


            visit “Navigation → BottomTabNavigator.tsx”


            <pre class=" CodeMirror-line">

import { Ionicons } from "@expo/vector-icons";
import { createBottomTabNavigator } from "@react-navigation/bottom-tabs";
import { createStackNavigator } from "@react-navigation/stack";
import * as React from "react";

import Colors from "../constants/Colors";
import useColorScheme from "../hooks/useColorScheme";
import TabOneScreen from "../screens/TabOneScreen";
import TabTwoScreen from "../screens/TabTwoScreen";
import TabThreeScreen from "../screens/TabThreeScreen";
import {
  BottomTabParamList,
  TabOneParamList,
  TabTwoParamList,
  TabThreeParamList
} from "../types";

const BottomTab = createBottomTabNavigator<BottomTabParamList>();

export default function BottomTabNavigator() {
  const colorScheme = useColorScheme();

  return (
    <BottomTab.Navigator
            initialRouteName="TabOne"
            tabBarOptions={{ activeTintColor: Colors[colorScheme].tint }}
    >
      <BottomTab.Screen
              name="Home"
              component={TabOneNavigator}
              options={{
              tabBarIcon: ({ color })=> (
            <TabBarIcon name="ios-code" color={color}/>
          )
        }}
      />
      <BottomTab.Screen
              name="New Transaction"
              component={TabTwoNavigator}
              options={{
              tabBarIcon: ({ color })=> (
            <TabBarIcon name="ios-code" color={color}/>
          )
        }}
      />
      <BottomTab.Screen
              name="Reports"
              component={TabThreeNavigator}
              options={{
              tabBarIcon: ({ color })=> (
            <TabBarIcon name="ios-code" color={color}/>
          )
        }}
      />
    </BottomTab.Navigator>
  );
}

// You can explore the built-in icon families and icons on the web at:
// https://icons.expo.fyi/
function TabBarIcon(props: { name: string; color: string }) {
  return <Ionicons size={30} style={{ marginBottom: -3 }} {...props}/>;
}

// Each tab has its own navigation stack, you can read more about this pattern here:
// https://reactnavigation.org/docs/tab-based-navigation#a-stack-navigator-for-each-tab
const TabOneStack = createStackNavigator<TabOneParamList>();

function TabOneNavigator() {
  return (
    <TabOneStack.Navigator>
      <TabOneStack.Screen
              name="TabOneScreen"
              component={TabOneScreen}
              options={{ headerTitle: "My Expenses" }}
      />
    </TabOneStack.Navigator>
  );
}

const TabTwoStack = createStackNavigator<TabTwoParamList>();

function TabTwoNavigator() {
  return (
    <TabTwoStack.Navigator>
      <TabTwoStack.Screen
              name="TabTwoScreen"
              component={TabTwoScreen}
              options={{ headerTitle: "New Transaction" }}
      />
    </TabTwoStack.Navigator>
  );
}

const TabThreeStack = createStackNavigator<TabThreeParamList>();

function TabThreeNavigator() {
  return (
    <TabThreeStack.Navigator>
      <TabThreeStack.Screen
              name="TabThreeScreen"
              component={TabThreeScreen}
              options={{ headerTitle: "Reports" }}
      />
    </TabThreeStack.Navigator>
  );
}
</pre>

            visit “Navigation → LinkingConfiguration.tsx”
            <pre class=" CodeMirror-line">
import * as Linking from "expo-linking";

export default {
  prefixes: [Linking.makeUrl("/")],
  config: {
    screens: {
      Root: {
        screens: {
          TabOne: {
            screens: {
              TabOneScreen: "one"
            }
          },
          TabTwo: {
            screens: {
              TabTwoScreen: "two"
            }
          },
          TabThree: {
            screens: {
              TabTwoScreen: "three"
            }
          }
        }
      },
      NotFound: "*"
    }
  }
};
</pre>


            visit “screens → TabOneScreen.tsx”
            <pre class=" CodeMirror-line">
import * as React from "react";
import { StyleSheet, ScrollView } from "react-native";

import EditScreenInfo from "../components/EditScreenInfo";
import { Text, View } from "../components/Themed";
import ExpenseList from "../components/custom/ExpenseList.tsx";

export default function TabOneScreen() {
  return (
    <View style={styles.container}>
      <Text style={styles.title}>Expense Tracker</Text>
      <View
              style={styles.separator}
              lightColor="#eee"
              darkColor="rgba(255,255,255,0.1)"
      />
      <EditScreenInfo path="/screens/TabOneScreen.tsx"/>
      <ScrollView style={styles.scrollView}>
        <ExpenseList/>
      </ScrollView>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    alignItems: "center",
    justifyContent: "center"
  },
  title: {
    marginTop: 20,
    fontSize: 20,
    fontWeight: "bold"
  },
  separator: {
    marginVertical: 30,
    height: 1,
    width: "80%"
  }
});
</pre>


            visit “screens → TabTwoScreen.tsx”
            <pre class=" CodeMirror-line">
import * as React from "react";
import { StyleSheet } from "react-native";

import EditScreenInfo from "../components/EditScreenInfo";
import { Text, View } from "../components/Themed";
import ExpenseForm from "../components/custom/ExpenseForm.tsx";

export default function TabTwoScreen() {
  return (
    <View
            style={{
            flex: 1
            }}
    >
      <Text style={styles.title}>New Transaction</Text>
      <View
              style={styles.separator}
              lightColor="#eee"
              darkColor="rgba(255,255,255,0.1)"
      />
      <ExpenseForm/>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    alignItems: "center",
    justifyContent: "center"
  },
  title: {
    fontSize: 20,
    marginTop: 20,
    marginLeft: 20,
    fontWeight: "bold"
  },
  separator: {
    marginVertical: 30,
    height: 1,
    marginLeft: 20,
    width: "80%"
  }
});
</pre>


            10. Create File “TabThreeScreen.tsx”

            “screens → TabThreeScreen.tsx”
            <pre class=" CodeMirror-line">
import * as React from "react";
import { StyleSheet } from "react-native";

import EditScreenInfo from "../components/EditScreenInfo";
import { Text, View } from "../components/Themed";
import ReportsList from "../components/custom/ReportsList.tsx";
import TodaysReport from "../components/custom/TodaysReport.tsx";
import YesterdaysReport from "../components/custom/YesterdaysReport.tsx";
import ThisWeek from "../components/custom/ThisWeek.tsx";
import ThisMonth from "../components/custom/ThisMonth.tsx";

export default function TabThreeScreen() {
  return (
    <View
            style={{
            flex: 1
            }}
    >
      <Text style={styles.title}>Reports</Text>
      <View
              style={styles.separator}
              lightColor="#eee"
              darkColor="rgba(255,255,255,0.1)"
      />
      <TodaysReport/>
      <YesterdaysReport/>
      <ThisWeek/>
      <ThisMonth/>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    alignItems: "center",
    justifyContent: "center"
  },
  title: {
    fontSize: 20,
    marginTop: 20,
    marginLeft: 20,
    fontWeight: "bold"
  },
  separator: {
    marginVertical: 30,
    height: 1,
    marginLeft: 20,
    width: "80%"
  }
});
</pre>

            11. we will create some more files

            “components → custom → ExpenseForm.tsx”
            <pre class=" CodeMirror-line">
import React, { Component } from "react";
import { useState } from "react";

import {
  TouchableHighlight,
  View,
  TextInput,
  StyleSheet,
  KeyboardAvoidingView,
  Picker,
  Button,
  Alert,
  Text
} from "react-native";
import DateTimePicker from "react-native-modal-datetime-picker";
import { formatDateTime } from "./utilities";

const createSomethingsMissingAlert = () =>
  Alert.alert(
    "Something is Missing",
    "Please Entyer Required Field Data",
    [
      {
        text: "OK",
        onPress: () => console.log("<<<<< Somethings Missing>>>>>> ")
      }
    ],
    { cancelable: false }
  );

const createFinishedAddingAlert = () =>
  Alert.alert(
    "Finished Adding",
    "Succesfully finished Adding",
    [
      {
        text: "OK",
        onPress: () => console.log("ffffffffffffffff finished adding>>>>>> ")
      }
    ],
    { cancelable: false }
  );

class ExpenseForm extends Component {
  constructor(props) {
    super(props);
    this.state = {
      dataSource: "",
      title: "",
      description: "",
      category: "--Select One--",
      subcategory: "",
      thedatetime: "",
      amount: 0
    };
  }

  handleDatePicked = thedatetime => {
    this.setState({
      thedatetime
    });

    this.handleDatePickerHide();
  };

  handleDatePickerHide = () => {
    this.setState({
      showDatePicker: false
    });
  };

  handleDatePress = () => {
    this.setState({
      showDatePicker: true
    });
  };

  updateValue(text, fields) {
    if (fields == "title") {
      this.setState({
        title: text
      });
    } else if (fields == "amount") {
      this.setState({
        amount: text
      });
    }
  }
  submit = () => {
    if (
      isEmpty(this.state.title) ||
      isEmpty(this.state.amount) ||
      isEmpty(this.state.thedatetime) ||
      this.state.category == "--Select One--"
    ) {
      createSomethingsMissingAlert();
    } else {
      let formData = new FormData();
      // let collection = {};
      formData.append("title", this.state.title);
      formData.append("amount", this.state.amount);
      formData.append("category", this.state.category);
      formData.append("date_time", this.state.thedatetime);

      console.log(formData);
      fetch("https://facebook-dev-comp-api.herokuapp.com/add_exp.php", {
        method: "POST",
        headers: {
          "Content-Type": "multipart/form-data."
        },
        body: formData
      })
        .then(response => response.json())
        .then(data => {
          console.log("Success:", data);
        })
        .catch(error => {
          console.error("Error:", error);
        }),
        this.setState({
          dataSource: "",
          title: "",
          description: "",
          category: "--Select One--",
          subcategory: "",
          thedatetime: "",
          amount: 0
        });
      createFinishedAddingAlert();
    }
  };

  render() {
    return (
      <View
              style={{
              flex: 1
              }}
      >
        <KeyboardAvoidingView
                behavior={Platform.OS == "ios" ? "padding" : "height"}
          style={styles.container}
        >
          <View style={styles.fieldContainer}>
            <TextInput
                    style={styles.text}
                    placeholder="Expense Title"
                    spellCheck={false}
                    name="myTitle"
                    value={this.state.title}
                    onChangeText={text => this.updateValue(text, "title")}
            />
          </View>
          <View style={styles.fieldContainer}>
            <TextInput
                    style={styles.text}
                    placeholder="Amount"
                    spellCheck={false}
                    keyboardType={"numeric"}
                    name="myAmount"
                    value={this.state.amount}
                    onChangeText={text => this.updateValue(text, "amount")}
            />
          </View>
          <View style={styles.fieldContainer}>
            <TextInput
                    style={[styles.text, styles.borderTop]}
                    placeholder="Event date"
                    spellCheck={false}
                    editable={!this.state.showDatePicker}
                    onFocus={this.handleDatePress}
                    value={formatDateTime(this.state.thedatetime)}
            />
            <DateTimePicker
                    isVisible={this.state.showDatePicker}
                    mode="datetime"
                    onConfirm={this.handleDatePicked}
                    onCancel={this.handleDatePickerHide}
            />
          </View>
          <View style={styles.pickerContainer}>
            <Picker
                    selectedValue={this.state.category}
                    style={{ height: 50, width: 200 }}
                    onValueChange={(itemValue, itemIndex)=>
                this.setState({ category: itemValue })
              }
            >
              <Picker.Item label="--Select One--" value="--Select One--"/>
              <Picker.Item label="Automobile" value="Automobile"/>
              <Picker.Item label="Clothing" value="Clothing"/>
              <Picker.Item label="Debt Reduction" value="Debt Reduction"/>
              <Picker.Item label="Education" value="Education"/>
              <Picker.Item
                      label="Entertainment/Fun"
                      value="Entertainment/Fun"
              />
              <Picker.Item label="Family" value="Family"/>
              <Picker.Item label="Food" value="Food"/>
              <Picker.Item label="Gifts" value="Gifts"/>
              <Picker.Item label="Giving" value="Giving"/>
              <Picker.Item
                      label="Household Items/Supplies"
                      value="Household Items/Supplies"
              />
              <Picker.Item label="Insurance" value="Insurance"/>
              <Picker.Item label="Investments" value="Investments"/>
              <Picker.Item label="Maintenance" value="Maintenance"/>
              <Picker.Item label="Medical" value="Medical"/>
              <Picker.Item label="Personal" value="Personal"/>
              <Picker.Item label="Shelter/Home" value="Shelter/Home"/>
              <Picker.Item label="Training" value="Training"/>
              <Picker.Item label="Transportation" value="Transportation"/>
              <Picker.Item label="Travel/Vacations" value="Travel/Vacations"/>
              <Picker.Item label="Utilities" value="Utilities"/>
            </Picker>
          </View>
          <TouchableHighlight onPress={this.submit} style={styles.button}>
            <Text style={styles.buttonText}>Add</Text>
          </TouchableHighlight>
          </KeyboardAvoidingView>
      </View>
    );
  }
}

const styles = StyleSheet.create({
  fieldContainer: {
    marginTop: 20,
    marginLeft: 20,
    marginRight: 20,
    backgroundColor: "#fff"
  },
  text: {
    height: 40,
    margin: 0,
    marginRight: 7,
    paddingLeft: 10
  },
  borderTop: {
    borderColor: "#edeeef",
    borderTopWidth: 0.5
  },
  button: {
    height: 50,
    backgroundColor: "#48BBEC",
    borderColor: "#48BBEC",
    alignSelf: "stretch",
    margin: 10,
    justifyContent: "center",
    alignItems: "center",
    borderRadius: 5
  },
  buttonText: {
    color: "#fff",
    fontSize: 18
  },
  pickerContainer: {
    flex: 1,
    paddingTop: 5,
    alignItems: "center"
  }
});

function isEmpty(obj) {
  return obj.length === 0;
}
function nulifyAll() {}
export default ExpenseForm;
</pre>


            “components → custom → ExpenseList.tsx”
            <pre class=" CodeMirror-line">
import React, { Component } from "react";
import {
  FlatList,
  Text,
  View,
  StyleSheet,
  ScrollView,
  ActivityIndicator
} from "react-native";
import Constants from "expo-constants";
import { createStackNavigator } from "@react-navigation/stack";
import { toCommaAmount } from "./utilities";

const Stack = createStackNavigator();

function MyStack() {
  return (
    <Stack.Navigator>
      <Stack.Screen name="Home" component={ExpenseList}/>
      <Stack.Screen name="NewTransaction" component={ExpenseForm}/>
    </Stack.Navigator>
  );
}

function Item({ title }) {
  return (
    <View style={styles.item}>
      <Text style={styles.title}>{title}</Text>
    </View>
  );
}

class ExpenseList extends Component {
  constructor(props) {
    super(props);
    this.state = {
      isLoading: true,
      dataSource: null
    };
  }

  componentDidMount() {
    return fetch("https://facebook-dev-comp-api.herokuapp.com/get_all.php")
      .then(response => response.json())
      .then(responseJson => {
        this.setState({
          isLoading: false,
          dataSource: responseJson.items
        });
      })

      .catch(error => console.log(error));
  }

  render() {
    if (this.state.isLoading) {
      return (
        <View style={styles.container}>
          <ActivityIndicator/>
        </View>
      );
    } else {
      let myExpenses = this.state.dataSource.map((val, key) => {
        return (
          <View key={key} style={styles.item}>
            <Text>
              {val.title} {toCommaAmount(val.amount)}
            </Text>
            <Text>{val.date_time}</Text>
          </View>
        );
      });

      return <View style={styles.container}>{myExpenses}</View>;
    }
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    marginTop: Constants.statusBarHeight,
    width: 250
  },
  item: {
    backgroundColor: "#f9c2ff",
    padding: 10,
    marginVertical: 4,
    marginHorizontal: 8
  },
  title: {
    fontSize: 16
  },
  scrollView: {
    marginHorizontal: 20
  }
});
export default ExpenseList;
</pre>


            “components → custom → ReportsList.tsx”
            <pre class=" CodeMirror-line">
import React, { Component } from "react";
import {
  FlatList,
  Text,
  View,
  StyleSheet,
  ScrollView,
  ActivityIndicator
} from "react-native";
import Constants from "expo-constants";
import { createStackNavigator } from "@react-navigation/stack";

const Stack = createStackNavigator();

function MyStack() {
  return (
    <Stack.Navigator>
      <Stack.Screen name="All Reports" component={ReportsList}/>
    </Stack.Navigator>
  );
}

function Item({ title }) {
  return (
    <View style={styles.item}>
      <Text style={styles.title}>{title}</Text>
    </View>
  );
}

class ReportsList extends Component {
  constructor(props) {
    super(props);
    this.state = {
      isLoading: true,
      dataSource: null
    };
  }

  componentDidMount() {
    return fetch("https://facebook-dev-comp-api.herokuapp.com/get_all.php")
      .then(response => response.json())
      .then(responseJson => {
        this.setState({
          isLoading: false,
          dataSource: responseJson.items
        });
      })

      .catch(error => console.log(error));
  }

  render() {
    if (this.state.isLoading) {
      return (
        <View style={styles.container}>
          <ActivityIndicator/>
        </View>
      );
    } else {
      let myExpenses = this.state.dataSource.map((val, key) => {
        return (
          <View key={key} style={styles.item}>
            <Text>
              {val.title} {val.amount}
            </Text>
          </View>
        );
      });

      return <View style={styles.container}>{myExpenses}</View>;
    }
  }
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    marginTop: Constants.statusBarHeight,
    width: 250
  },
  item: {
    backgroundColor: "#f9c2ff",
    padding: 10,
    marginVertical: 4,
    marginHorizontal: 8
  },
  title: {
    fontSize: 16
  },
  scrollView: {
    marginHorizontal: 20
  }
});
export default ReportsList;
</pre>


            The next file is a function that handles a few general functions and repetitive activities

            “components → custom → utilities.tsx”
            <pre class=" CodeMirror-line">
import moment from "moment";

export function formatDate(dateString) {
  const parsed = moment(new Date(dateString));

  if (!parsed.isValid()) {
    return dateString;
  }

  return parsed.format("D MMM YYYY");
}

export function formatDateTime(dateString) {
  const parsed = moment(new Date(dateString));

  if (!parsed.isValid()) {
    return dateString;
  }

  return parsed.format("H A on D MMM YYYY");
}

export function getCountdownParts(eventDate) {
  const duration = moment.duration(
    moment(new Date(eventDate)).diff(new Date())
  );
  return {
    days: parseInt(duration.as("days")),
    hours: duration.get("hours"),
    minutes: duration.get("minutes"),
    seconds: duration.get("seconds")
  };
}

export function toCommaAmount(strOrig) {
  console.log("<<<<<<<<<<<INSIDE TO COMMA AMOUNT>>>>>>>>>>>>>");
  if (strOrig === null) {
    console.log("<<<<<<<<<<<strOrig IS NULLLLLLLL>>>>>>>>");
  } else {
    let strLen = strOrig.length;
    console.log("strLen >>", strLen);
    let builder = "";
    let newamt = "";
    // Initialize StringBuilder with this value.
    if (strOrig.includes(".")) {
      strLen = strLen - 3;
      if (strLen < 4) {
        newamt = strOrig;
      }

      if (strLen == 4) {
        builder = strOrig.slice(0, 1) + "," + strOrig.slice(1, strLen);
        newamt = builder;
      }
      if (strLen == 5) {
        builder = strOrig.slice(0, 2) + "," + strOrig.slice(2, strLen);
        newamt = builder;
      }

      if (strLen == 6) {
        builder = strOrig.slice(0, 3) + "," + strOrig.slice(3, strLen);
        newamt = builder;
      }

      if (strLen == 7) {
        builder =
          strOrig.slice(0, 1) +
          "," +
          strOrig.slice(1, 5) +
          "," +
          strOrig.slice(4, strLen);
        newamt = builder;
      }
      if (strLen == 8) {
        builder =
          strOrig.slice(0, 2) +
          "," +
          strOrig.slice(2, 6) +
          "," +
          strOrig.slice(5, strLen);
        newamt = builder;
      }
      if (strLen == 9) {
        builder =
          strOrig.slice(0, 3) +
          "," +
          strOrig.slice(3, 7) +
          "," +
          strOrig.slice(6, strLen);
        newamt = builder;
      }

      if (strLen == 10) {
        builder =
          strOrig.slice(0, 1) +
          "," +
          strOrig.slice(1, 5) +
          "," +
          strOrig.slice(4, 8) +
          "," +
          strOrig.slice(7, strLen);
        newamt = builder;
      }
      if (strLen == 11) {
        builder =
          strOrig.slice(0, 2) +
          "," +
          strOrig.slice(2, 6) +
          "," +
          strOrig.slice(5, 9) +
          "," +
          strOrig.slice(8, strLen);
        newamt = builder;
      }
    } else {
      if (strLen < 4) {
        newamt = strOrig;
      }

      if (strLen == 4) {
        builder = strOrig.slice(0, 1) + "," + strOrig.slice(1, strLen);
        newamt = builder;
      }
      if (strLen == 5) {
        builder = strOrig.slice(0, 2) + "," + strOrig.slice(2, strLen);
        newamt = builder;
      }

      if (strLen == 6) {
        builder = strOrig.slice(0, 3) + "," + strOrig.slice(3, strLen);
        newamt = builder;
      }

      if (strLen == 7) {
        builder =
          strOrig.slice(0, 1) +
          "," +
          strOrig.slice(1, 5) +
          "," +
          strOrig.slice(4, strLen);
        newamt = builder;
      }
      if (strLen == 8) {
        builder =
          strOrig.slice(0, 2) +
          "," +
          strOrig.slice(2, 6) +
          "," +
          strOrig.slice(5, strLen);
        newamt = builder;
      }
      if (strLen == 9) {
        builder =
          strOrig.slice(0, 3) +
          "," +
          strOrig.slice(3, 7) +
          "," +
          strOrig.slice(6, strLen);
        newamt = builder;
      }

      if (strLen == 10) {
        builder =
          strOrig.slice(0, 1) +
          "," +
          strOrig.slice(1, 5) +
          "," +
          strOrig.slice(4, 8) +
          "," +
          strOrig.slice(7, strLen);
        newamt = builder;
      }
      if (strLen == 11) {
        builder =
          strOrig.slice(0, 2) +
          "," +
          strOrig.slice(2, 6) +
          "," +
          strOrig.slice(5, 9) +
          "," +
          strOrig.slice(8, strLen);
        newamt = builder;
      }
    }

    return "N" + newamt;
  }
}
</pre>

            12. Finally we make changes to App.tsx

            “App.tsx”
            <pre class=" CodeMirror-line">
import { StatusBar } from "expo-status-bar";
import React from "react";
import { SafeAreaProvider } from "react-native-safe-area-context";

import useCachedResources from "./hooks/useCachedResources";
import useColorScheme from "./hooks/useColorScheme";
import Navigation from "./navigation";

export default function App() {
  const isLoadingComplete = useCachedResources();
  const colorScheme = useColorScheme();

  if (!isLoadingComplete) {
    return null;
  } else {
    return (
      <SafeAreaProvider>
        <Navigation colorScheme={colorScheme}/>
        <StatusBar/>
      </SafeAreaProvider>
    );
  }
}
</pre>


            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>this is how the app will finally look</span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><img src="https://exp-trkr.herokuapp.com/img/5.jpg" width="149" height="256" name="Image6" align="left" border="0"/>
                <img src="https://exp-trkr.herokuapp.com/img/6.jpg" width="149" height="256" name="Image7" align="left" border="0"/></p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
            <ol>
                <ol start="6">
                    <li>
                        <h2 class="western">Final Words</h2>
                    </li>
                </ol>
            </ol>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Hurraaay! we made it. Our Expense tracker is ready and fully functional.</span></span></span>
            </p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>Many thanks to those awesome guys at Facebook for making this great tool called React Native and don t forget to visit the really helpful official React Native documentation website from our trusted pals at Facebook using the below link</span></span></span>
            </p>
            <p class="western">https://github.com/techlinesolutions/expense</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>I hope you enjoyed reading this as much as I enjoyed preparing it. If you have any questions or comments don't forget to reach out. Happy Tracking :)</span></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western"><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span>All the code is available in below github repo</span></span></span>
            </p>
            <p class="western"><span style="color: #000080;"><span lang="zxx"><u><span style="color: #333333;"><span
                    style="font-family: Roboto, Arial, sans-serif;"><span><a href="https://github.com/techlinesolutions/expense" target="_blank">https://github.com/techlinesolutions/expense</a></span></span></span></u></span></span>
            </p>
            <p class="western">&nbsp;</p>
            <p class="western">&nbsp;</p>
##License
          
ExpensTracker is distributed under the <a href="http://opensource.org/licenses/MIT" target="_blank">MIT Open source license</a>.</span></span></span>
 
        </div>
    </div>
</div>

