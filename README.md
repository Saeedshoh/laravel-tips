# Советы по Laravel
Советы по Laravel

 * [Сгенерировать пароль во время создание пользователя](#set_password)



<a name="set_password"></a> 
##### Сгенерировать пароль во время создание пользователя

    public function setPasswordAttribute($password)
    {
        if($password != null) {
            $this->attributes['password'] = bcrypt($password);
        }
    }
    
    
    
    
    
