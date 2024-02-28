# PowerShell
# Get Computer Name
$computerName = $env:COMPUTERNAME

# Get Logged-in User
$loggedInUser = $env:USERNAME

# Get IP Address
$ipAddress = (Test-Connection -ComputerName $computerName -Count 1).IPv4Address.IPAddressToString

# Output Results
Write-Host "Computer Name: $computerName"
Write-Host "Logged-in User: $loggedInUser"
Write-Host "IP Address: $ipAddress"
