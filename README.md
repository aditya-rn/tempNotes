# Bluetooth Service Configuration

This document describes the supported Bluetooth services and their characteristics used in the application. The configuration is defined in the `SUPPORTED_SERVICES` array, which specifies the UUIDs for services and their corresponding read/write characteristics.

## Supported Services Array

The `SUPPORTED_SERVICES` array contains configurations for two different Bluetooth services. Here's the complete array for reference:

```typescript
export const SUPPORTED_SERVICES: SupportedService[] = [
  {
    serviceUUID: '442f1570-8a00-9a28-cbe1-e1d4212d53eb',
    readCharacteristicUUID: '442f1571-8a00-9a28-cbe1-e1d4212d53eb',
    writeCharacteristicUUID: '442f1572-8a00-9a28-cbe1-e1d4212d53eb',
  },
  {
    serviceUUID: '0000ffe0-0000-1000-8000-00805f9b34fb',
    readCharacteristicUUID: '0000ffe1-0000-1000-8000-00805f9b34fb',
    writeCharacteristicUUID: '0000ffe1-0000-1000-8000-00805f9b34fb',
  },
];
```

## Service 1 Configuration

Service UUID:
```
442f1570-8a00-9a28-cbe1-e1d4212d53eb
```

Read Characteristic UUID:
```
442f1571-8a00-9a28-cbe1-e1d4212d53eb
```

Write Characteristic UUID:
```
442f1572-8a00-9a28-cbe1-e1d4212d53eb
```

## Service 2 Configuration

Service UUID:
```
0000ffe0-0000-1000-8000-00805f9b34fb
```

Read/Write Characteristic UUID:
```
0000ffe1-0000-1000-8000-00805f9b34fb
```

Note: For Service 2, the same UUID is used for both read and write characteristics.

## Type Definition

The array uses the following TypeScript interface:

```typescript
interface SupportedService {
  serviceUUID: string;
  readCharacteristicUUID: string;
  writeCharacteristicUUID: string;
}
```

Each service configuration includes:
- `serviceUUID`: The UUID of the Bluetooth service
- `readCharacteristicUUID`: The UUID of the characteristic used for reading data
- `writeCharacteristicUUID`: The UUID of the characteristic used for writing data
