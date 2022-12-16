# ideapad_acpi
Ideapad gaming 3(15ach6)


#Charge battery Full:

```sh
echo 0 | sudo tee /sys/bus/platform/drivers/ideapad_acpi/VPC2004\:00/conservation_mode
```

#Charge battery till 60%:

```sh
echo 1 | sudo tee /sys/bus/platform/drivers/ideapad_acpi/VPC2004\:00/conservation_mode
```

#Fan Profiles:

> 0 -> Super Silent Mode
> 1 -> Standard Mode
> 2 -> Dust Cleaning
> 4 -> Efficient Thermal Dissipation Mode

```sh
echo 1 | sudo tee /sys/bus/platform/drivers/ideapad_acpi/VPC2004\:00/fan_mode
```
