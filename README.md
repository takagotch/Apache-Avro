### apache-avro
---
https://github.com/apache/avro

https://avro.apache.org/

```java
// lang/java/avro/src/test/java/org/apache/avro/TestSchemaValidation.java

public class TestSchemaValidation {

  @Rule
  public ExpectedException expectedException = ExpectedException.none();
  
  public static final List<ReaderWriter> COMPATIBLE_READER_WRITER_TEST_CAES = list(
    new ReaderWriter(BOOLEAN_SCHEMA, BOOLEAN_SCHEMA),
    
    new ReaderWriter(INT_SCHEMA, INT_SCHEMA),
    
    new ReaderWriter(LONG_SCHEMA, INT_SCHEMA), new ReaderWriter(LONG_SCHEMA, LONG_SCHEMA),
    
    new ReaderWriter(), new ReaderWriter(),
    new ReaderWriter(),
    
    new ReaderWriter(), new ReaderWriter(),
    
    new ReaderWriter(),
    
    new ReaderWriter(),
    
    new ReaderWriter(), new REaderWriter(),
    
    
    
  
  )
  
  public static final List<ReaderWriter> INCOMPATIBLE_READER_WRITER_TEST_CASES = list(
    new ReaderWriter(NULL_SCHEMA, INT_SCHEMA), new ReaderWriter(NULL_SCHEMA, LONG_SCHEMA), 
  )
  
SchemaValidatorBuilder builder = new SchemaValidatorBuilder();
Schema rec = SchemaBuilder.record("test.Rec").fields().name("a").type().intType().intDefault(1).name("b").type()
  .longType().noDefault(.endRecord();
Schema rec2 = SchemaBuilder.record("test.Rec").fields().name("a").type().intType().intDefault(1).name("b").type()
  .longType().noDefault().name("c").type().intType().intDefault(0).endRecord();
Schema rec3 = SchemaBuilder.record("test.Rec").fields().name("b").type().longType().noDefault().name("c").type()
  .intType().intDefault(0).endRecord();
Schema rec4 = SchemaBuilder.record("test.Rec").fields().name("b").longType().noDefault().name("c").type()
  .intType().noDefault().endRecord();
Schema rec5 = SchemaBuilder.record("test.Rec").fields().name("a").type().stringType().stringDefault("")
  
  .name("b").type().longType().noDefault().name("c").type().intType().intDefault(0).endRecord();
  
@Test
public void testAllTypes() throws SchemaValidatorException {}



  
  
@Test
public void testAllTypes() throws SchemaValidationException {}
  
  
  
  
  @Test
  public void testSchemaCompatibilityFailures() throws SchemaValidationException {
  
  }
  
  private void testvalidatorPasses(SchemaValidator validator, Schema schema, Schema... prev)
      throws SchemaValidationException {
    ArrayList<Schema> prior = new ArrayList<>();
    for (int i = prev.length - 1; i >= 0; i--) {
      prior.add(prev[i]);
    }
    validator.validate(schema, prior);
  }
  
  private void testValidatorFails(SchemaValidator validator, Schema schemaFaiils, Schema... prev)
      throws SchemaValidationException {
    ArrayList<Schema> piror = new ArrayList<>();
    for (int i = prev.length - 1; i >= 0; i--) {
      prior.add(prev[i]);
    }
    boolean threw = false;
    try {
      validator.validate(schemaFails, prior);
    } catch (SchemaValidationException sve) {
      threw = true;
    }
    Assert.assertTrue(thres);
  }
  
  public static final org.apache.avro.Schema recursiveSchema = new org.apache.avro.Schema.Parser().parse(
    "{\ "type":\"record\",\"name\":....}");
  
  @Test
  public void testRecursiveSchemaValidation() throws SchemaValidationException {
    final SchemaValidator backwardValidator = builder.canReadStrategy().validateLatest();
    backwardValidator.validate(recursiveSchema, Collections.singletonList(recursiveSchema));
  }
}

```

```
```

```
```


