Configuration Manager & Chat Service
This project demonstrates two patterns:

Singleton Pattern for managing global configurations.

Adapter Pattern for integrating a legacy chat service into a modern system.

Project Structure:
Configuration Manager (Singleton Pattern)
ConfigurationManager.java: Manages global settings like max players, default language, and difficulty.

ConfigManagerDemo.java: Demonstrates how to use the ConfigurationManager.

Chat Service (Adapter Pattern)
LegacyChatService.java: A simple legacy chat service.

ChatService.java: The modern interface for sending messages.

ChatServiceAdapter.java: Adapts the legacy chat service to the modern interface.

ChatAdapterDemo.java: Demonstrates how to use the adapter.


📝 What the Code Does
Configuration Manager (Singleton Pattern)
Singleton Pattern:

The ConfigurationManager class has a private constructor, so you can't create an instance from outside.

The getInstance() method returns the single instance of the class. If it doesn't exist, it creates one.

Setting Configurations:

Use methods like setMaxplayer, setDeflanguage, and setDifficult to add settings.

Getting Configurations:

Use the getConfig method to get a value by its key.

Printing All Configurations:

The printAllConfigs method shows all the settings in a clear format.

Chat Service (Adapter Pattern)
Legacy Chat Service:

The LegacyChatService class has a method sendLegacyMessage that prints messages in a specific format.

Modern Chat Service Interface:

The ChatService interface defines a method sendMessage for sending messages.

Adapter:

The ChatServiceAdapter class adapts the legacy chat service to the modern interface.

Demo:

The ChatAdapterDemo class shows how to use the adapter to send messages.
