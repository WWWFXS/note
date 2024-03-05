
#### 1.ClassPathXmlApplicationContext
    public ClassPathXmlApplicationContext(String configLocation) throws BeansException {
		this(new String[] {configLocation}, true, null);
	}
--------
     public ClassPathXmlApplicationContext(
			String[] configLocations, boolean refresh, @Nullable ApplicationContext parent)
			throws BeansException {

		super(parent);
		setConfigLocations(configLocations);
		if (refresh) {
			refresh();
		}
	}
 -------------
 ###### super(parent);
      public AbstractXmlApplicationContext(@Nullable ApplicationContext parent) {
		super(parent);
	}
###### super(parent);
    public AbstractRefreshableConfigApplicationContext(@Nullable ApplicationContext parent) {
		super(parent);
	}
###### 	super(parent);
    public AbstractApplicationContext(@Nullable ApplicationContext parent) {
		this();
		setParent(parent);
	}
###### this();
    public AbstractApplicationContext() {
		this.resourcePatternResolver = getResourcePatternResolver();
	}
        
    

    


