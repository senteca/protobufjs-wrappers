## How to use the custom loader with NestJS

```
npm i -S @sentecacommerce/protobufjs-wrappers
```

```typescript
app.connectMicroservice<MicroserviceOptions>({
  transport: Transport.GRPC,
  options: {
    url: '0.0.0.0:443',
    package: 'package.name',
    protoPath: join(__dirname, 'path_to_proto'),
    protoLoader: '@sentecacommerce/protobufjs-wrappers',
  },
});
```

## Supported types

- `google.protobuf.Struct`
- `google.protobuf.Timestamp`
