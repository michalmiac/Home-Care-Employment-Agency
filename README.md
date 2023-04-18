# Home Care Employment Agency

+ [Network cluster](https://github.com/michalmiac/Agencja-pracy/edit/main/README.md#se%C4%87-komputerowa)
+ [VoIP technical solutions](https://github.com/michalmiac/Agencja-pracy/edit/main/README.md#rozwi%C4%85zania-techniczne-voip)
+ [Office management software](https://github.com/michalmiac/Agencja-pracy/edit/main/README.md#oprogramowanie-do-obs%C5%82ugi-biura)


In my employment agency, which specializes in providing caregivers for elderly people in their own homes, the field of IT plays a crucial role. Based on specialized software developed by me, we were able to effectively manage and organize the work of our employees and provide full administrative support for the office.
My IT solutions allow for easy and fast management of orders, assigning caregivers to specific clients, monitoring task completion, and generating reports. All these features are available in a clear and intuitive graphical interface, designed with the comfort and efficiency of my employees in mind.
In addition to solutions directly related to order management, the software also includes special tools for the recruitment department, allowing for quick and precise recruitment processes and complete documentation of employees.
All of these IT solutions are constantly being developed and improved by me to meet the demands of our clients and ensure the best quality of services in the field of elderly care.

# Network cluster
![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/20230407_174626.jpg)
The presented photo shows a network cluster in the testing phase. On the left side, there are servers that act as file servers, backups, databases, and backends for office management applications. On the right and bottom, WiFi routers, a switch, and a Cisco router are visible. All devices in the office, including computers, printers, and monitoring devices, are connected to a central point that separates and secures connections, providing the necessary bandwidth for the most efficient operation of the complex infrastructure.
+ Installation of the **Ubuntu Server** system image on the **Raspberry** device, as a stable and familiar system structure
  + Use of the **MongoDB** database due to its **JSON** format for aggregating objects from the Java language
  + Utilization of **SpringBoot** as the REST server
  + Access to the file server via the **SSH** protocol. External graphical access to files through the **SFTP** protocol in the file explorer window in Ubuntu
  + Use of the **Bacula** program for creating backups
  + Remote access to resources through the **OpenVPN** technology


# VoIP technical solutions
![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/20230407_164237.jpg)
In the above image, the electronic components are visible in sequence from the left side: a step-down converter, a SIM800L GSM/GPRS module, connectors exiting the module to a board with resistors that lead to an Audio Jack connection, and finally a sound card. By connecting the SIM800L module to a computer via a serial port, it is possible to control the module, send commands for sending and receiving text messages (SMS), and issue commands to initiate voice calls. A Java program was specifically created for this project, enabling the sending of ATM commands via the serial port to the GSM board, allowing for the exchange of text messages through the same channel. Meanwhile, the sound that reaches the GSM module is passed through the resistors to the Audio Jack connection, and then to the sound card. Sending sound to the GSM module works in precisely the opposite way, where the sound card sends the sound to the Audio Jack connection, and then it passes through the resistors to the GSM board, allowing for sound exchange. An important element in the presented sound connection is the sending of ATM commands to initiate a call, but of course, it is equally important to be able to receive sound and send sound from the sound card. Another Java program was written for this purpose.
# Office management software
### Below are graphical representations of some modules of the office task management program. They are only a small sample of the available functionalities, and their purpose is to provide a general overview of the tasks that our company faces.

![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Steilen-Personal-Care-FRONTEND-(2).svg)



![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2015-44-34.png)

Above is the welcome screen of the program. The employee can choose whether to log into the system. Depending on the user's location, the program offers a choice of database connection types.

![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2012-51-18.png)
On the first image, which appears after the user logs in, there is a graphical interface allowing for adding, deleting, and displaying employees from the contact database. The central element of the interface is a table presenting a list of contacts, which enables filtering and sorting of results according to various criteria, such as language proficiency or gender. Such functionalities are extremely important for the company as they allow finding employees who are perfectly matched to the needs of clients, such as elderly people requiring care. The employee database, which is included in the graphical interface, thus constitutes the most important resource of the company.

![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2014-15-04.png)
The image shows a window used to save employee contact information in the database. The options available during data entry are extremely important from a recruitment standpoint, allowing for a thorough evaluation of a candidate's qualifications to meet client requirements. For example, preferences regarding smoking can be specified. Additionally, a benefit is the ability to record conversations with the employee, which ensures the ability to retrieve necessary information from past conversations. As a result, the contact-saving window is an extremely useful tool for the company, enabling precise selection of employees to meet customer needs.


![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2012-53-26.png)
The next module presented is the one used for calculating employee salaries. This tool aims to facilitate the process of calculating salaries and prevent errors that may occur when manually calculating wages. This process is very complex and requires taking into account various aspects, such as the exact start time of work, the currency of the paid salary, deductions for transport or enforcement, and also converting these payments into different currencies. A big advantage of this module is the ability to generate calculations in the form of a PDF protocol, which allows them to be sent to employees so that they can thoroughly review each step of their salary calculation.


![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2012-53-47.png)
The next window presents a module for assigning and tracking tasks assigned to office employees. This is an extremely important tool because it allows not only for assigning tasks to specific employees, but also for tracking the stages of their completion. Each employee has the ability to monitor tasks assigned to them and save necessary information regarding their execution. Thanks to this module, office work becomes more efficient and organized, and employees can effectively carry out their assigned tasks.
![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2012-54-12.png)
The image shows a module that allows for the creation of a personal questionnaire for caregivers. This tool makes it easy to collect and store important information about our employees. It is worth emphasizing that the generated form can be exported to a PDF format, which allows for easy sending to our clients at a later stage of the recruitment process. Thanks to this, our clients can familiarize themselves with preliminary information about potential caregivers and choose the best candidate for their care.
![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2012-55-02.png)
The above module allows for searching transports for transporting our employees to their workplace. Due to the fact that our employees reside in virtually all areas of Poland, there is a database of carriers taking into account the areas they serve in their transport services. Thanks to this tool, it is possible to significantly shorten the time of searching for carriers compared to the traditional method of calling each of them.
![My animated logo](https://github.com/michalmiac/Agencja-pracy/blob/main/graphics/Screenshot%20from%202023-04-07%2015-15-16.png)
W tym ujęciu przedstawiony jest moduł odpowiedzialny za przechowywanie dokumentów, zleceń oraz informacji zebranych z całego programu zatrudnionych pracowników. Dzięki temu modułowi możemy automatycznie generować dokumenty w formacie PDF, takie jak umowy, zlecenia podróży, ewidencję czasu pracy oraz różnego rodzaju raporty. Istnieje możliwość śledzenia, gdzie dokładnie znajdują się dokumenty w danym momencie po ich wysłaniu do pracownika, na przykład przez tradycyjną pocztę. Jednym z ważnych elementów tego modułu jest możliwość przeglądania informacji na temat dokumentów, które wymagają opracowania, uzupełnienia, złożenia lub wysłania. Moduł "informacje" stanowi centralne miejsce gromadzenia danych z całego programu dotyczących rzeczy, które są jeszcze do należy podjąć w odniesieniu dla danego pracownika.


### Below are code snippets of the software used for office task management. These snippets showcase the technical solutions applied in the application. The code has been designed to increase programming efficiency and ensure greater application performance and scalability. These solutions make application development more intuitive, programming easier, and faster.

```java
default Object createDto(Object dtoObject, Object controllerClass, @Nullable List<?> list, @Nullable String ARRAY_NAME) throws IOException {
    ObjectMapper mapper = new ObjectMapper();
    ObjectNode jsonNode = mapper.createObjectNode();

    for (Field field : controllerClass.getClass().getDeclaredFields()) {
        if (field.isAnnotationPresent(MyAnno.class)) {
            field.setAccessible(true);
            try {
                Object value = field.get(controllerClass);

                if (value == null) {
                    jsonNode.putNull(field.getName());
                } else {
                    switch (field.getType().getCanonicalName()) {
                        case "javafx.scene.control.TextField":
                            jsonNode.put(field.getName(), ((TextField) value).getText());
                            break;
                        case "javafx.scene.control.DatePicker":
                            LocalDate dateValue = ((DatePicker) value).getValue();
                            jsonNode.put(field.getName(), dateValue != null ? dateValue.toString() : null);
                            break;
                        case "javafx.scene.control.ChoiceBox":
                            jsonNode.put(field.getName(), ((ChoiceBox<?>) value).getValue().toString());
                            break;
                        case "javafx.scene.control.CheckBox":
                            jsonNode.put(field.getName(), ((CheckBox) value).isSelected());
                            break;
                        case "javafx.scene.control.TextArea":
                            jsonNode.put(field.getName(), ((TextArea) value).getText());
                            break;
                        case "java.lang.String":
                            jsonNode.put(field.getName(), (String) value);
                            break;
                        default:
                            throw new IllegalArgumentException("Unsupported field type: " + field.getType().getCanonicalName());
                    }
                }
            } catch (IllegalAccessException e) {
                e.printStackTrace();
            }
        }
    }

    if (list != null && !list.isEmpty()) {
        ArrayNode arrayNode = mapper.createArrayNode();
        for (Object scheduleInfoDto : list) {
            String scheduleInfoJson = mapper.writeValueAsString(scheduleInfoDto);
            arrayNode.add(mapper.readTree(scheduleInfoJson));
        }
        jsonNode.set(ARRAY_NAME, arrayNode);
    }

    dtoObject = mapper.treeToValue(jsonNode, dtoObject.getClass());
    return dtoObject;
}
```    
This code aims to enable scalability by using the MyAnno annotation, which allows for freely specifying the fields from which the value should be extracted. This makes it easy to add new fields without having to modify the createDto method.    
+ ObjectNode was used to store keys and values in JSON format.
+ The accessibility of private fields was set by using field.setAccessible(true).
+ An additional null value checking to avoid exceptions was added.
+ A switch statement with explicit values for field types, which avoids the need to use the instanceof method.


```java
private static final Map<Class<?>, Consumer<Object>> HANDLERS = new HashMap<>();

static {
    HANDLERS.put(Button.class, controller -> {
        Button button = (Button) controller;
        button.setOnAction(event -> buttonEventHandleInterfaceHandler.handle());
    });
    HANDLERS.put(CheckBox.class, controller -> {
        CheckBox checkBox = (CheckBox) controller;
        checkBox.setOnAction(event -> eventHandleInterfaceHandler.handle());
    });
    HANDLERS.put(ChoiceBox.class, controller -> {
        ChoiceBox choiceBox = (ChoiceBox) controller;
        choiceBox.setOnAction(event -> eventHandleInterfaceHandler.handle());
    });
}

public static void setEventHandlerOnAllElements(Object controllerClass, EventHandleInterfaceHandler eventHandleInterfaceHandler, ButtonEventHandleInterfaceHandler buttonEventHandleInterfaceHandler) {
    Arrays.stream(controllerClass.getClass().getFields())
            .filter(field -> field.isAnnotationPresent(MyAnno.class))
            .forEach(field -> {
                Class<?> fieldType = field.getType();
                if (HANDLERS.containsKey(fieldType)) {
                    try {
                        Object fieldObject = field.get(controllerClass);
                        HANDLERS.get(fieldType).accept(fieldObject);
                    } catch (IllegalAccessException e) {
                        e.printStackTrace();
                    }
                }
            });
}
```
    
The above code aims to facilitate the handling of events for multiple user interface elements in a JavaFX controller. The MyAnno annotation was created specifically for this purpose and is used to mark fields in the controller class that are intended for event handling. As per the code, only fields marked with this annotation will be processed in the setEventHandlerOnAllElements method. This approach can simplify user interface programming by allowing the definition of fields to be used for event handling and then quickly and easily processing them throughout the controller class.
